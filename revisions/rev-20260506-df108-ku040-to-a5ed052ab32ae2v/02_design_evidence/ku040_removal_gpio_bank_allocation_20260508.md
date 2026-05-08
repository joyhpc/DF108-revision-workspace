# KU040 Removal And Decoder GPIO Bank Allocation - 2026-05-08

本文件记录 2026-05-08 新增设计输入：目标第一版原理图中 `KU040` 需要完全删除；从解码板过来的 `168` 个普通 GPIO 需要接入电压可调 I/O bank，可调范围为 `1.2 V` 到 `1.8 V`。

本文件是快速第一版原理图推进证据，不是 pinout sign-off、发板批准或正式设计冻结。

## 当前设计状态

| 分类 | 状态 |
|---|---|
| 已确认 | `U14 = XCKU040-2FFVA1156I` 不再作为 dual-option 保留，目标第一版应删除 KU040 主控域 |
| 已确认 | 解码板到主控板新增 `168` 路普通 GPIO，非 MIPI/高速通道 |
| 已确认 | 这 `168` 路 GPIO 需要放在支持 `1.2 V` 到 `1.8 V` 的可调 I/O bank |
| 暂定假设 | 当前画图仍按 `A5EC052A B32A` 占位 pinout 组织，但 A5EC/A5ED 差异不再只是命名问题 |
| 待补证 | Quartus exact device、Pin Planner、最终 A5EC/A5ED ordering code、解码板连接器 pin map、GPIO 方向/复用/电平时序 |
| 当前要画的页 | `SCH_A5E_SYMBOL`、`SCH_DECODER_GPIO_VADJ`、`SCH_POWER_TREE`、`SCH_CLOCK_RESET_CONFIG` |

## 技术层

### 1. KU040 删除口径

第一版目标原理图不再保留 `U14 KU040` 作为双主控或兼容选项。

画图时应按以下原则处理：

- 旧 KU040 的 DDR4、configuration、clock/reset、电源 rails 和专用控制链路从目标主控域中移除。
- 旧 KU040 承担的外部接口 owner 必须重新归属到 Agilex 5、解码板、MCU、外设保持域或明确删除。
- 不能再用“U14 与 U9 共存”解释重复电源、重复控制线和重复接口 owner。

### 2. 168 路普通 GPIO 的 bank 类型选择

这批 GPIO 需要 `1.2 V` 到 `1.8 V` 可调电压，因此第一选择是 Agilex 5 `HSIO` bank 的 `VCCIO_PIO` 供电域。

根据本地 Agilex 5 General-Purpose IO User Guide 文本证据：

- HSIO bank 的 `VCCIO_PIO` 供电，每个 I/O sub-bank 只有一个 I/O voltage。
- HSIO 支持 `1.2 V LVCMOS`，也支持 `1.8 V` 相关 I/O 标准。
- 未使用 HSIO sub-bank 默认可能被 Quartus 分配为 `1.2 V`，但本设计不能依赖默认值，必须显式约束。

不建议把这批 `1.2 V` 到 `1.8 V` 可调 GPIO 放到 `HVIO`：

- HVIO 面向高电压普通 I/O，局部资料口径显示为 `1.8 V / 2.5 V / 3.3 V` 类用途。
- 若必须支持 `1.2 V`，应优先使用 HSIO/VCCIO_PIO，而不是 HVIO。

### 3. Bank 容量判断

本地 pinout JSON 显示：

| 占位器件 | HSIO 可用 sub-bank | HSIO GPIO 容量 | 结论 |
|---|---:|---:|---|
| `A5EC052A_B32A` | `8` 个，每个 `48` pins | `384` pins | 原始数量上可以容纳 168 GPIO，但还要避开 LPDDR5 EMIF 和 MIPI |
| `A5ED052A_B32A` | `4` 个，每个 `48` pins | `192` pins | 168 GPIO 会占用几乎全部 HSIO，基本无法同时容纳两组 LPDDR5 x32 和 MIPI |

因此，A5EC/A5ED 在本问题上不再只是命名清理项。若最终必须使用 `A5ED052AB32AE2V`，需要用 Quartus exact device / Pin Planner 重新证明 bank 数量和资源是否足够。

### 4. 第一版推荐分组

168 路普通 GPIO 建议先按 `4` 个可调电压 GPIO group 组织：

| Group | GPIO 数 | 目标 bank 类型 | 目标供电 | 第一版画图动作 |
|---|---:|---|---|---|
| `DEC_GPIO_VADJ_G0` | `42` | HSIO / VCCIO_PIO sub-bank | `VADJ_GPIO_0` 或公共 `VADJ_GPIO` | 画到 Agilex 5 GPIO bank 占位页，pin 待 Pin Planner |
| `DEC_GPIO_VADJ_G1` | `42` | HSIO / VCCIO_PIO sub-bank | `VADJ_GPIO_1` 或公共 `VADJ_GPIO` | 画到 Agilex 5 GPIO bank 占位页，pin 待 Pin Planner |
| `DEC_GPIO_VADJ_G2` | `42` | HSIO / VCCIO_PIO sub-bank | `VADJ_GPIO_2` 或公共 `VADJ_GPIO` | 画到 Agilex 5 GPIO bank 占位页，pin 待 Pin Planner |
| `DEC_GPIO_VADJ_G3` | `42` | HSIO / VCCIO_PIO sub-bank | `VADJ_GPIO_3` 或公共 `VADJ_GPIO` | 画到 Agilex 5 GPIO bank 占位页，pin 待 Pin Planner |

每个 HSIO sub-bank 有 `48` 个 single-ended I/O pins。按每组 `42` 路分配时，每个 bank 保留 `6` 路余量，用于后续补齐控制、spare、调试、方向修正或 Pin Planner 逃逸调整。

### 5. 候选 bank 分配

第一版不要直接把 `168` 个 GPIO 锁到具体球脚。建议先在原理图中使用逻辑 bank label：

```text
DEC_GPIO_VADJ_G0 -> GPIO_VADJ_BANK0 -> HSIO/VCCIO_PIO sub-bank TBD
DEC_GPIO_VADJ_G1 -> GPIO_VADJ_BANK1 -> HSIO/VCCIO_PIO sub-bank TBD
DEC_GPIO_VADJ_G2 -> GPIO_VADJ_BANK2 -> HSIO/VCCIO_PIO sub-bank TBD
DEC_GPIO_VADJ_G3 -> GPIO_VADJ_BANK3 -> HSIO/VCCIO_PIO sub-bank TBD
```

若继续按 `A5EC052A B32A` 占位推进，可优先让 Pin Planner 尝试把 GPIO 放入不影响 LPDDR5/MIPI 的 `4` 个 HSIO sub-bank。候选池包括：

```text
2A_B, 2A_T, 2B_B, 2B_T, 3A_B, 3A_T, 3B_B, 3B_T
```

其中 `3A_T` 是 SDM shared HSIO，正式使用前必须确认配置模式和 SDM 资源限制。

若最终 `A5ED052A_B32A` pinout 只剩 `2A_B / 2A_T / 2B_B / 2B_T` 四个 HSIO sub-bank，则这四个 bank 被 168 GPIO 基本吃满，不建议继续把 MIPI 与两组 LPDDR5 x32 同时压进同一器件方案。此时应在以下路径中选一种：

- 改回或确认使用具备足够 HSIO 的 A5EC-like 器件；
- 把部分普通 GPIO 下放到解码板侧 MCU / GPIO expander / CPLD / bridge；
- 减少普通 GPIO 数量或固定到 `1.8 V` 后评估 HVIO 可用性；
- 重新评估两组 LPDDR5 x32 或 MIPI 资源占用；
- 换更大封装/不同器件资源组合。

### 6. 原理图页面处理建议

`SCH_DECODER_GPIO_VADJ` 页建议画成四个相同结构：

```text
Decoder connector GPIO[0:41]    -> DEC_GPIO_VADJ_G0 -> GPIO_VADJ_BANK0
Decoder connector GPIO[42:83]   -> DEC_GPIO_VADJ_G1 -> GPIO_VADJ_BANK1
Decoder connector GPIO[84:125]  -> DEC_GPIO_VADJ_G2 -> GPIO_VADJ_BANK2
Decoder connector GPIO[126:167] -> DEC_GPIO_VADJ_G3 -> GPIO_VADJ_BANK3
```

每组页面至少标注：

- connector pin map: TBD
- GPIO direction: input/output/bidirectional TBD
- bank voltage: `1.2 V` to `1.8 V`, controlled by `VADJ_GPIO` rail plan
- exact A5E bank/pin: pending Pin Planner
- relation to MIPI/LPDDR5: must not consume EMIF or MIPI required banks

## 决策层

KU040 删除会让所有旧主控 GPIO 归属问题变成真实迁移工作，不能再用“双方案共存”解释。

168 路可调电压普通 GPIO 的数量很大。按 A5EC 占位器件看，原始 HSIO 数量有机会承接；按 A5ED 本地 pinout 看，它会吃掉几乎全部 HSIO，和 MIPI、两组 LPDDR5 x32 明显冲突。

当前第一版最稳妥的画法是：先画四组 `DEC_GPIO_VADJ_G0..G3` 逻辑 bank，占位到 HSIO/VCCIO_PIO；不要写死球脚。下一步必须用 Quartus exact device + Pin Planner 同时放入 `MIPI + 2x LPDDR5 x32 + 168 GPIO`，否则这个架构不能进入正式冻结。
