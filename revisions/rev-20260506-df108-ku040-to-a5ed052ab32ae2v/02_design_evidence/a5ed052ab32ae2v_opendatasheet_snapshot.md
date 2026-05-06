# A5ED052AB32AE2V Opendatasheet Snapshot

本文件是从本地 `opendatasheet` 已有导出抽取的器件证据快照。它是 borrowed evidence，不是 Intel 官方 last-mile 复核结论。

## 1. 型号映射

| 字段 | 当前识别 |
|---|---|
| 用户给定完整型号 | `A5ED052AB32AE2V` |
| 本地结构化导出 | `A5ED052A_B32A.json` |
| device | `A5ED052A` |
| package | `B32A` |
| family | `Agilex 5` |
| series | `E-Series` |
| role | `FPGA SoC` |
| HPS | quad |
| transceiver | true |
| crypto | true |

判断：当前导出可以支持 `A5ED052A + B32A` 的结构化审查准备；完整 ordering code 的 `E2V` 尾缀仍需官方订购码资料复核。

## 2. 资源快照

| 资源 | 数值 |
|---|---:|
| logic elements | 523920 |
| ALM | 177600 |
| M20K count | 1288 |
| M20K Mbit | 25.16 |
| MLAB count | 8440 |
| MLAB Mbit | 5.15 |
| DSP count | 1352 |
| INT8 TOPS | 20.78 |
| pins | 1591 |
| power rails | 54 |
| banks | 22 |
| diff pairs | 156 |

## 3. 高速与接口能力

| 能力块 | 当前导出 |
|---|---|
| GTS RX lane pairs | 24 |
| GTS TX lane pairs | 24 |
| refclk pair count | 12 |
| quad count | 6 |
| max rate | 28.1 Gbps |
| supported protocols | PCIe 4.0, 10G Ethernet, 25G Ethernet, custom |
| PCIe x4 hard IP instances | 6 |
| gigabit ethernet MAC/PCS count | 4 |
| HVIO count | 120 |
| HSIO count | 384 |
| HPS IO count | 48 |
| MIPI D-PHY interface count | 28 |
| external memory | DDR4, DDR5, LPDDR4, LPDDR5 |
| x32 memory interface count | 4 |
| HPS cores | Arm Cortex-A76, Arm Cortex-A55 |

对 DF108 当前约束的初步含义：

- 40G 光口如果按 4 x 10G 组织，GTS lane 数量和速率在资源层面有基础。
- 8 路 FAKRA/POC/DPS 是外设域保持约束，当前还不能仅凭器件资源判断通过，必须等原理图导出后做接口保持矩阵。
- HPS 引入会影响上电、复位、配置、固件升级和控制路径，后续必须进入 MCM-G2/MCM-G3 gate。

## 4. 来源追溯

| 对象 | 来源 |
|---|---|
| package pinout | `a5ed052a.xlsx`, Intel document `830449` |
| package pinout source version | `2025-06-06` |
| package pinout source status | Final |
| device capability | `agilex5_device_overview_762191_2024_09_06` |
| ordering variant | `agilex5_part_number_decoder_762191_2024_09_06` |

## 5. 需要人工复核的点

| 项 | 原因 | 状态 |
|---|---|---|
| `A5ED052AB32AE2V` 的完整订购码分解 | 本地导出只明确 `A5ED052A_B32A`，未完整覆盖 `E2V` 尾缀 | open |
| Power rail 电压、容差、sequencing | 当前快照只有 pin/rail 名称与 pin count，不等价于电源设计规格 | open |
| HPS 是否启用 | 影响控制 MCU 替代、boot、升级和复位架构 | open |
| GTS lane / quad / refclk 分配 | 影响 40G 光口、PCIe/Ethernet/custom protocol 可行性 | open |
| 旧 DF108 外设域保持 | 需要当前/旧版原理图差异和物理接口约束 | blocked by schematic intake |
