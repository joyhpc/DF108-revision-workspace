# Current Design Direction Update - 2026-05-07

本文件记录 2026-05-07 新增的设计输入与当前建议方向。

它是改版过程证据，不是原理图 sign-off、发板批准或正式设计冻结。

## 0. 新增设计输入

| 项 | 用户输入 | 当前处理口径 |
|---|---|---|
| MIPI | 去掉 HS/LP 切换开关，去掉 buffer；MIPI 从解码板经过连接器后直连 Agilex 5 | 作为新的主路径架构处理 |
| 主芯片侧连接 | 全部连接到 `A5EC052A B32A` 的 HSIO bank | 按当前占位器件与封装口径处理，正式命名前仍需校核 |
| 存储 | DDR4 改为 LPDDR5 | 需进入 EMIF pin/bank/resource gate |
| 电源入口 | 使用已有成熟 LM5060 方案 | 电路结构可迁移，参数按新负载重新核算 |
| 参考文件 | Google Drive: `1LBmcH09JFtY-A9iW-TYNtksNjdZ7o8wS` | 已可匿名下载并抽取关键 PDF 条目；PDF 不进入 GitHub |

## 1. MIPI 架构判断

### 技术层

建议采用以下拓扑：

```text
Decoder board MIPI D-PHY
  -> board-to-board connector
  -> DF108 main board controlled-impedance routing
  -> A5EC052A B32A MIPI-capable HSIO bank
  -> Agilex 5 MIPI D-PHY IP
```

设计判断：

- 去掉 HS/LP 切换开关和 buffer 是合理方向。
- Agilex 5 原生 MIPI D-PHY 支持 high-speed 与 low-power signaling，不应再在板级额外做 HS/LP 切换。
- 该接口不能按普通差分 IO 处理，必须按 MIPI D-PHY IP 的 placement、RZQ、refclk、bank 和 lane 规则处理。
- 对 Agilex 5 E-Series Group A 口径，MIPI D-PHY high-speed 速率按以下边界设计：
  - short / standard reference channel: up to `3.5 Gbps/lane`
  - long reference channel 或损耗较大链路: up to `2.5 Gbps/lane`
- 板间连接器、跨板走线、插损、阻抗连续性、lane skew 会决定能否按 `3.5 Gbps/lane` 闭合。

待验证项：

- 解码板输出是否为标准 MIPI D-PHY CSI-2 电气接口，而不是私有并口或经过桥接的非标准物理层。
- 每路 lane 数、lane rate、clock lane、virtual channel 与 Agilex 5 MIPI IP 配置是否一致。
- 连接器和主板走线是否满足目标速率下的通道损耗和 skew 要求。
- MIPI HSIO bank 与 LPDDR5 EMIF bank 是否发生 byte lane、sub-bank、RZQ 或 refclk 资源冲突。

### 决策层

MIPI 直连方案可以降低板级复杂度，减少切换器和 buffer 带来的信号完整性风险，也减少调试变量。

主要风险从“板上切换电路是否正确”转移为“Agilex 5 HSIO/MIPI pin 规划和跨板高速通道是否满足速率”。因此下一步不应先画完整原理图，而应先冻结 MIPI lane map 与 HSIO bank 资源表。

## 2. LPDDR5 速率与架构判断

### 技术层

基于用户提供的 Agilex 5 参考文件，本阶段按 `A5EC052A B32A` / Agilex 5 E-Series Group A 口径处理：

| 项 | 建议采用的设计口径 |
|---|---:|
| LPDDR5 controller | hard memory controller |
| LPDDR5 clock | `1,866.667 MHz` |
| LPDDR5 per-pin data rate | `3,733 Mbps/pin` |
| 最大数据宽度口径 | `x32` |
| `x16` raw bandwidth | about `7.46 GB/s` |
| `x32` raw bandwidth | about `14.93 GB/s` |

注意：

- EMIF IP 参数中可见更高枚举频点不等于 `A5EC052A B32A` 实际可用上限。
- 本阶段不要把 `2,750 MHz / 5,500 Mbps` 当作 A5EC052A 的可闭合设计目标。
- 原理图和 layout 应按 `3,733 Mbps/pin` 能力设计；bring-up 可从低 FSP 档启动，再升到目标频率。
- 实际有效带宽取决于访问模式、refresh、仲裁、burst 效率和 fabric/HPS 数据路径，不能直接等同 raw bandwidth。

推荐执行路径：

1. 先在 Quartus EMIF IP 中选择 exact device / package / speed grade。
2. 生成 LPDDR5 x32 或 2ch x16 的候选 pinout。
3. 用 pin planner 检查 EMIF bank、RZQ、refclk、address/command lane、data byte lane 是否合法。
4. 再回填原理图符号分页和连接器/走线规划。
5. 原理图 review 前必须把 LPDDR5 vendor datasheet、package pinout、termination/ODT、reset、ZQ/RZQ 规则纳入证据。

### 决策层

LPDDR5 可以作为 DDR4 替代方向，但它不是简单换料。它会重写存储 bank 资源、pinout、约束、layout 规则和 bring-up 策略。

对当前项目，建议把 `3,733 Mbps/pin` 作为设计目标上限，把 `x32` 或 `2ch x16` 作为候选架构。若系统带宽预算不要求满速，可在调试和量产配置中选择更保守的运行档位，提高裕量。

## 3. LM5060 电源入口迁移判断

### 技术层

LM5060 输入方案可按成熟电路迁移，但参数不能原样假定闭合。

迁移时至少复核：

- DC24V 输入范围、浪涌、反接/过压保护边界。
- UV/OV 阈值和迟滞是否适合 DF108 当前输入规范。
- sense resistor、current limit、timer、dv/dt、inrush profile。
- 外置 MOSFET 的 SOA、热设计和故障工况。
- TVS、保险丝、EMI 滤波和连接器前后级保护。
- `PG` / `FLT` 信号如何进入新的 Agilex 5 power sequencing。
- 后级总输入电容和所有 POL 的启动浪涌是否超过旧 LM5060 参数裕量。

### 决策层

LM5060 是低风险复用块，但不是零工作量迁移。它的价值是保留成熟的 24V 热插拔/保护入口；主要新增工作是按 Agilex 5 + LPDDR5 新电源树重算启动电流和故障保护裕量。

## 4. 当前推荐总体架构

```text
DF108 external domain
  FAKRA / POC / DPS / enclosure / optical physical form factor preserved

Decoder board domain
  MAX96712 / DS90UB9702 / other decoder-side devices
  MIPI D-PHY output preserved if protocol/electrical interface matches

Main controller board
  DC24V input
    -> mature LM5060 hot-swap/protection block
    -> new Agilex 5 power tree and sequencing

  MIPI from decoder board
    -> connector
    -> direct controlled-impedance routing
    -> A5EC052A B32A MIPI-capable HSIO banks

  External memory
    -> LPDDR5 hard memory controller
    -> x32 or 2ch x16 candidate topology
    -> target design rate 3,733 Mbps/pin
```

## 5. 下一步必须冻结的表

在继续画主控原理图前，应先冻结一张 `A5EC052A B32A resource allocation matrix`：

| 资源域 | 必填内容 | gate 目的 |
|---|---|---|
| MIPI | decoder source, connector pins, lane count, lane rate, A5EC bank/lane pins, clock lane, RZQ/refclk | 防止 MIPI 直连路径画错 bank |
| LPDDR5 | component topology, x16/x32/2ch x16, EMIF bank, byte lane, address/command lane, RZQ, reset, refclk | 防止 EMIF pinout 不合法 |
| Power | LM5060 output, POL list, rail voltage/tolerance/current, sequencing, PG/FLT chain | 防止旧电源入口与新电源树不匹配 |
| Clock/reset | MIPI refclk, EMIF refclk, system reset, configuration reset, power-good dependencies | 防止上电链路不可 bring-up |
| Naming | A5EC/A5ED placeholder rule, final order code, symbol value, BOM value, PST export value | 防止临时名称进入正式发布 |

## 6. 参考资料

用户提供的参考文件夹：

- `https://drive.google.com/drive/folders/1LBmcH09JFtY-A9iW-TYNtksNjdZ7o8wS?dmr=1&ec=wgc-drive-%5Bmodule%5D-goto`

已下载并用于本文件判断的主要文件：

- `Agilex 5 FPGAs and SoCs Device Overview ug-762191-762192.pdf`
- `Agilex 5 FPGAs and SoCs Device Data Sheet-ds-813918-813919.pdf`
- `External Memory Interfaces (EMIF) IP User Guide Agilex 5 FPGAs and SoCs 817467_D842785.pdf`
- `General-Purpose IO User Guide Agilex 5 FPGAs and SoCs 813934_869633.pdf`
- `MIPI D-PHY IP User Guide 817561_856924.pdf`
- `altera-pbc-b32a-a5e.xlsx`

本文件引用这些资料作为过程证据。正式原理图冻结前仍需用最新 Intel/Altera 官方文档、Quartus device/pin planner、EMIF IP 输出和 memory vendor datasheet 做 last-mile 校核。
