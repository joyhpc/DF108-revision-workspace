# A38 Agilex 5 High-Speed And Decoder GPIO Allocation - 2026-05-12

本文件记录 A38 / DF108 `KU040 -> Agilex 5` Rev1 原理图设计中，高速接口和解码板 GPIO 的当前第一版分配建议。

本文件是设计过程证据和画图输入，不是 pinout sign-off、EMIF closure、SI closure、发板批准或正式冻结结论。

## 当前设计状态

```text
已确认:
- 目标 Rev1 删除旧 U14 KU040 主控路径。
- J5/J6/J7/J8 为 10144518-102802LF，每个连接器承载 2 个解码通道。
- 解码板普通控制 GPIO 共 168 路，需要接到支持 1.2 V 到 1.8 V 可调的 Agilex 5 I/O bank。

暂定假设:
- MIPI 从解码板经 10144518-102802LF 连接器直连 Agilex 5 MIPI-capable HSIO。
- 旧 DDR4 改为 2 组 x32 LPDDR5，每组一个 LPDDR5 hard memory controller。
- QSFP 光口物理形态保留，高速差分对接 Agilex 5 GTS transceiver。

待补证:
- Quartus exact device / Pin Planner 同时放入 MIPI、2 x LPDDR5 x32、QSFP GTS 和 168 GPIO。
- MIPI lane placement、RZQ/refclk、目标速率和通道损耗。
- LPDDR5 EMIF bank、byte lane、RZQ、refclk、vendor pinout。
- QSFP GTS lane / quad / refclk 分配和低速控制电平。

当前要画的页:
- SCH_MIPI_DIRECT
- SCH_LPDDR5_CTRL0 / SCH_LPDDR5_CTRL1
- SCH_QSFP_GTS
- SCH_DECODER_GPIO_VADJ
```

## 技术层

### 1. 证据来源

| 项 | 来源 |
|---|---|
| revision | `rev-20260506-df108-ku040-to-a5ed052ab32ae2v` |
| netlist | `01_inputs/raw/normalized_for_intake/pstxnet.dat` |
| BOM | `01_inputs/raw/normalized_for_intake/A38_MAIN_V1_2_A1_3.BOM` |
| 连接器 | `J5/J6/J7/J8 = 10144518-102802LF` |
| QSFP | `CON2 = QSFP` |
| 旧 DDR | `U3/U4/U5/U6 = DDR4-16-96P` |
| 当前 Agilex 占位 | `U9 = A5EC052A B32A` |
| 目标器件名 | `A5ED052AB32AE2V`, pending final package/resource proof |

### 2. 高速接口分配

| 域 | 当前连接器/器件 | 数量 | Agilex 5 目标资源 | 第一版动作 |
|---|---|---:|---|---|
| MIPI | J5/J6/J7/J8 | 8 组，每组 `CLK + D0..D3`，共 40 对差分 | MIPI-capable HSIO + MIPI D-PHY IP | 直连 Agilex 5，删除旧 HS/LP switch 和 buffer；exact lane pending Pin Planner |
| LPDDR5 | 替代旧 U3-U6 DDR4 | 2 组 x32 | LPDDR5 hard memory controller x2 | 先画 `LPDDR5_CTRL0_X32` / `LPDDR5_CTRL1_X32`，EMIF pinout 由 Quartus 生成 |
| QSFP | CON2 | 4 TX 对 + 4 RX 对 | GTS transceiver | 保留光口物理形态；lane/quad/refclk pending Quartus / reference design |

### 3. MIPI 连接器统计

每个解码通道使用 5 对 MIPI D-PHY 差分信号：`CLK`、`D0`、`D1`、`D2`、`D3`。

| Connector | Channels | MIPI pins | 说明 |
|---|---|---:|---|
| J5 | A/B | 20 | A: pins 3/5/9/11/15/17/21/23/27/29; B: pins 41/43/47/49/53/55/59/61/65/67 |
| J6 | C/D | 20 | C: pins 4/6/10/12/16/18/22/24/28/30; D: pins 42/44/48/50/54/56/60/62/66/68 |
| J7 | E/F | 20 | E follows A pattern; F follows B pattern |
| J8 | G/H | 20 | G follows C pattern; H follows D pattern |
| Total | A-H | 80 pins / 40 pairs | 8 groups x 5 differential pairs |

MIPI bank/pin 禁止在原理图第一版写死到普通差分 IO。必须等 MIPI D-PHY IP、RZQ、refclk、lane placement 和 SI channel budget 确认。

### 4. Decoder GPIO 总数和 bank 分配

每个解码通道有 21 路普通控制 GPIO：

```text
*_I2C1_SCL, *_I2C1_SDA
*_I2C2_SCL, *_I2C2_SDA
*_GPIO0..5
*_INT_RES
*_FSYNC
*_PWDN
*_IC_SEL
*_POC_PWR_SEL
*_MODE0, *_MODE1
*_ERRB
*_LOCK
*_IDX
*_LED
```

8 个通道共 `8 x 21 = 168` 路。这些信号全部按可调 `1.2 V` 到 `1.8 V` GPIO 处理，目标为 Agilex 5 HSIO / `VCCIO_PIO` sub-bank，不建议放入只适合固定高电压域的 HVIO。

| Group | Connector | Channels | GPIO count | Target | Voltage rail |
|---|---|---|---:|---|---|
| `DEC_GPIO_VADJ_G0` | J5 | A/B | 42 | one HSIO / VCCIO_PIO sub-bank | `VADJ_DEC_GPIO_G0` |
| `DEC_GPIO_VADJ_G1` | J6 | C/D | 42 | one HSIO / VCCIO_PIO sub-bank | `VADJ_DEC_GPIO_G1` |
| `DEC_GPIO_VADJ_G2` | J7 | E/F | 42 | one HSIO / VCCIO_PIO sub-bank | `VADJ_DEC_GPIO_G2` |
| `DEC_GPIO_VADJ_G3` | J8 | G/H | 42 | one HSIO / VCCIO_PIO sub-bank | `VADJ_DEC_GPIO_G3` |

如果系统确认所有 168 路 GPIO 永远同电压，可在电源页把 `VADJ_DEC_GPIO_G0..G3` 合并为公共 `VADJ_DEC_GPIO`。在未确认前，不要把四组直接短接成固定 1.8 V。

### 5. J5 GPIO pin map: channels A/B

| Signal role | A net / pin | B net / pin |
|---|---|---|
| I2C1_SCL | `A_I2C1_SCL` / J5.4 | `B_I2C1_SCL` / J5.42 |
| I2C1_SDA | `A_I2C1_SDA` / J5.6 | `B_I2C1_SDA` / J5.44 |
| I2C2_SCL | `A_I2C2_SCL` / J5.8 | `B_I2C2_SCL` / J5.46 |
| I2C2_SDA | `A_I2C2_SDA` / J5.10 | `B_I2C2_SDA` / J5.48 |
| GPIO0 | `A_GPIO0` / J5.12 | `B_GPIO0` / J5.50 |
| GPIO1 | `A_GPIO1` / J5.14 | `B_GPIO1` / J5.52 |
| GPIO2 | `A_GPIO2` / J5.16 | `B_GPIO2` / J5.54 |
| GPIO3 | `A_GPIO3` / J5.18 | `B_GPIO3` / J5.56 |
| GPIO4 | `A_GPIO4` / J5.20 | `B_GPIO4` / J5.58 |
| GPIO5 | `A_GPIO5` / J5.22 | `B_GPIO5` / J5.60 |
| INT_RES | `A_INT_RES` / J5.24 | `B_INT_RES` / J5.62 |
| FSYNC | `A_FSYNC` / J5.26 | `B_FSYNC` / J5.64 |
| PWDN | `A_PWDN` / J5.28 | `B_PWDN` / J5.66 |
| IC_SEL | `A_IC_SEL` / J5.30 | `B_IC_SEL` / J5.68 |
| POC_PWR_SEL | `A_POC_PWR_SEL` / J5.32 | `B_POC_PWR_SEL` / J5.70 |
| MODE0 | `A_MODE0` / J5.33 | `B_MODE0` / J5.71 |
| ERRB | `A_ERRB` / J5.34 | `B_ERRB` / J5.72 |
| MODE1 | `A_MODE1` / J5.35 | `B_MODE1` / J5.73 |
| LOCK | `A_LOCK` / J5.36 | `B_LOCK` / J5.74 |
| IDX | `A_IDX` / J5.37 | `B_IDX` / J5.75 |
| LED | `A_LED` / J5.38 | `B_LED` / J5.76 |

### 6. J6 GPIO pin map: channels C/D

| Signal role | C net / pin | D net / pin |
|---|---|---|
| I2C1_SCL | `C_I2C1_SCL` / J6.3 | `D_I2C1_SCL` / J6.41 |
| I2C1_SDA | `C_I2C1_SDA` / J6.5 | `D_I2C1_SDA` / J6.43 |
| I2C2_SCL | `C_I2C2_SCL` / J6.7 | `D_I2C2_SCL` / J6.45 |
| I2C2_SDA | `C_I2C2_SDA` / J6.9 | `D_I2C2_SDA` / J6.47 |
| GPIO0 | `C_GPIO0` / J6.11 | `D_GPIO0` / J6.49 |
| GPIO1 | `C_GPIO1` / J6.13 | `D_GPIO1` / J6.51 |
| GPIO2 | `C_GPIO2` / J6.15 | `D_GPIO2` / J6.53 |
| GPIO3 | `C_GPIO3` / J6.17 | `D_GPIO3` / J6.55 |
| GPIO4 | `C_GPIO4` / J6.19 | `D_GPIO4` / J6.57 |
| GPIO5 | `C_GPIO5` / J6.21 | `D_GPIO5` / J6.59 |
| INT_RES | `C_INT_RES` / J6.23 | `D_INT_RES` / J6.61 |
| FSYNC | `C_FSYNC` / J6.25 | `D_FSYNC` / J6.63 |
| PWDN | `C_PWDN` / J6.27 | `D_PWDN` / J6.65 |
| IC_SEL | `C_IC_SEL` / J6.29 | `D_IC_SEL` / J6.67 |
| POC_PWR_SEL | `C_POC_PWR_SEL` / J6.31 | `D_POC_PWR_SEL` / J6.69 |
| ERRB | `C_ERRB` / J6.33 | `D_ERRB` / J6.71 |
| MODE0 | `C_MODE0` / J6.34 | `D_MODE0` / J6.72 |
| LOCK | `C_LOCK` / J6.35 | `D_LOCK` / J6.73 |
| MODE1 | `C_MODE1` / J6.36 | `D_MODE1` / J6.74 |
| LED | `C_LED` / J6.37 | `D_LED` / J6.75 |
| IDX | `C_IDX` / J6.38 | `D_IDX` / J6.76 |

### 7. J7 GPIO pin map: channels E/F

| Signal role | E net / pin | F net / pin |
|---|---|---|
| I2C1_SCL | `E_I2C1_SCL` / J7.4 | `F_I2C1_SCL` / J7.42 |
| I2C1_SDA | `E_I2C1_SDA` / J7.6 | `F_I2C1_SDA` / J7.44 |
| I2C2_SCL | `E_I2C2_SCL` / J7.8 | `F_I2C2_SCL` / J7.46 |
| I2C2_SDA | `E_I2C2_SDA` / J7.10 | `F_I2C2_SDA` / J7.48 |
| GPIO0 | `E_GPIO0` / J7.12 | `F_GPIO0` / J7.50 |
| GPIO1 | `E_GPIO1` / J7.14 | `F_GPIO1` / J7.52 |
| GPIO2 | `E_GPIO2` / J7.16 | `F_GPIO2` / J7.54 |
| GPIO3 | `E_GPIO3` / J7.18 | `F_GPIO3` / J7.56 |
| GPIO4 | `E_GPIO4` / J7.20 | `F_GPIO4` / J7.58 |
| GPIO5 | `E_GPIO5` / J7.22 | `F_GPIO5` / J7.60 |
| INT_RES | `E_INT_RES` / J7.24 | `F_INT_RES` / J7.62 |
| FSYNC | `E_FSYNC` / J7.26 | `F_FSYNC` / J7.64 |
| PWDN | `E_PWDN` / J7.28 | `F_PWDN` / J7.66 |
| IC_SEL | `E_IC_SEL` / J7.30 | `F_IC_SEL` / J7.68 |
| POC_PWR_SEL | `E_POC_PWR_SEL` / J7.32 | `F_POC_PWR_SEL` / J7.70 |
| MODE0 | `E_MODE0` / J7.33 | `F_MODE0` / J7.71 |
| ERRB | `E_ERRB` / J7.34 | `F_ERRB` / J7.72 |
| MODE1 | `E_MODE1` / J7.35 | `F_MODE1` / J7.73 |
| LOCK | `E_LOCK` / J7.36 | `F_LOCK` / J7.74 |
| IDX | `E_IDX` / J7.37 | `F_IDX` / J7.75 |
| LED | `E_LED` / J7.38 | `F_LED` / J7.76 |

### 8. J8 GPIO pin map: channels G/H

| Signal role | G net / pin | H net / pin |
|---|---|---|
| I2C1_SCL | `G_I2C1_SCL` / J8.3 | `H_I2C1_SCL` / J8.41 |
| I2C1_SDA | `G_I2C1_SDA` / J8.5 | `H_I2C1_SDA` / J8.43 |
| I2C2_SCL | `G_I2C2_SCL` / J8.7 | `H_I2C2_SCL` / J8.45 |
| I2C2_SDA | `G_I2C2_SDA` / J8.9 | `H_I2C2_SDA` / J8.47 |
| GPIO0 | `G_GPIO0` / J8.11 | `H_GPIO0` / J8.49 |
| GPIO1 | `G_GPIO1` / J8.13 | `H_GPIO1` / J8.51 |
| GPIO2 | `G_GPIO2` / J8.15 | `H_GPIO2` / J8.53 |
| GPIO3 | `G_GPIO3` / J8.17 | `H_GPIO3` / J8.55 |
| GPIO4 | `G_GPIO4` / J8.19 | `H_GPIO4` / J8.57 |
| GPIO5 | `G_GPIO5` / J8.21 | `H_GPIO5` / J8.59 |
| INT_RES | `G_INT_RES` / J8.23 | `H_INT_RES` / J8.61 |
| FSYNC | `G_FSYNC` / J8.25 | `H_FSYNC` / J8.63 |
| PWDN | `G_PWDN` / J8.27 | `H_PWDN` / J8.65 |
| IC_SEL | `G_IC_SEL` / J8.29 | `H_IC_SEL` / J8.67 |
| POC_PWR_SEL | `G_POC_PWR_SEL` / J8.31 | `H_POC_PWR_SEL` / J8.69 |
| ERRB | `G_ERRB` / J8.33 | `H_ERRB` / J8.71 |
| MODE0 | `G_MODE0` / J8.34 | `H_MODE0` / J8.72 |
| LOCK | `G_LOCK` / J8.35 | `H_LOCK` / J8.73 |
| MODE1 | `G_MODE1` / J8.36 | `H_MODE1` / J8.74 |
| LED | `G_LED` / J8.37 | `H_LED` / J8.75 |
| IDX | `G_IDX` / J8.38 | `H_IDX` / J8.76 |

### 9. QSFP mapping

CON2 保留为 QSFP 物理光口。高速差分对建议接 Agilex 5 GTS：

| QSFP side | Nets |
|---|---|
| TX pairs | `SFP0_TX_P/N`, `SFP1_TX_P/N`, `SFP2_TX_P/N`, `SFP3_TX_P/N` |
| RX pairs | `SFP0_RX_P_R/N_R`, `SFP1_RX_P_R/N_R`, `SFP2_RX_P_R/N_R`, `SFP3_RX_P_R/N_R` |
| Low-speed control | `QSFP_MODSELL`, `QSFP_RESETL`, `QSFP_LPMODE`, `QSFP_INTL`, `QSFP_MODPRSL`, `QSFP_SCL`, `QSFP_SDA` |
| Power | `VCCR`, `VCCT`, `VCC1` |

QSFP 低速控制不应与 168 路解码板 VADJ GPIO 混为同一个电压域，除非模块侧电平和 pull-up rail 已确认兼容。

### 10. Resource placement order

第一版画图和 Pin Planner 放置顺序建议：

1. `LPDDR5_CTRL0_X32` / `LPDDR5_CTRL1_X32`: 先锁定 EMIF hard controller、byte lane、RZQ、refclk。
2. QSFP GTS: 锁定 GTS quad、lane polarity、refclk 和 AC coupling。
3. MIPI D-PHY: 放置 8 组 MIPI lane，确认 MIPI-capable HSIO、RZQ、refclk。
4. `DEC_GPIO_VADJ_G0..G3`: 放入剩余可用 HSIO / VCCIO_PIO sub-bank。

这样做的原因是 LPDDR5、QSFP、MIPI 的 placement 自由度低，普通 GPIO 的可搬迁性最高。

## 决策层

当前第一版可以继续画，但不能宣布资源闭合。

对项目经理而言，风险集中在两个点：

| 风险 | 业务影响 |
|---|---|
| `A5ED052AB32AE2V` B32A 若只有 4 个可用 HSIO sub-bank | 168 路可调 GPIO 会几乎吃满 HSIO，MIPI 和 2 组 LPDDR5 x32 可能无法同时成立，导致器件/封装/GPIO 架构返工 |
| MIPI + LPDDR5 + QSFP 都依赖工具确认 | 原理图可以先出第一版，但正式冻结前必须补 Quartus/Pin Planner/Fitter 证据，否则后续 PCB 可能返工 |

推荐决策：

- 继续画 Rev1 原理图，但把 `DEC_GPIO_VADJ_G0..G3` 作为逻辑 bank 占位，不锁死 Agilex 5 球脚。
- 立即做一次 Quartus exact device 资源试放：`MIPI + 2x LPDDR5 x32 + QSFP GTS + 168 GPIO`。
- 如果 A5ED B32A 资源不足，优先在项目层面决策：换 A5EC-like/更大封装、减少 GPIO、固定部分 GPIO 到 1.8 V 后评估 HVIO、或把部分 GPIO 下放到解码板侧 CPLD/expander。
