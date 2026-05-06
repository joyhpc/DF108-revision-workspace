# Source vs Target Chip Check

本文件记录当前输入原理图与用户目标型号之间的第一轮一致性检查。

## 技术层

| 检查对象 | 证据 | 结果 |
|---|---|---|
| 用户目标型号 | `A5ED052AB32AE2V` | target |
| BOM 新增 Agilex 器件 | `A38_MAIN_V1_2_A1_3.BOM:126` 显示 `U9 A5EC052A B32A` | mismatch |
| BOM 旧 FPGA | `A38_MAIN_V1_2_A1_3.BOM:129` 显示 `U14 XCKU040-2FFVA1156I` | old KU040 still present |
| pstchip 旧 FPGA | `pstchip.dat` 中 `VALUE='XCKU040-2FFVA1156I'` | old KU040 still present |
| pstchip 新 FPGA | `pstchip.dat` 中 `PART_NAME='A5EC052A B32A'`, `VALUE='A5EC052A B32A'` | mismatch with target A5ED |

## A5EC vs A5ED 差异

| 项 | A5EC052A_B32A | A5ED052A_B32A |
|---|---|---|
| variant_code | C | D |
| device_role | FPGA | FPGA SoC |
| HPS | none | quad |
| transceiver | true | true |
| crypto | false | true |

判断：如果项目真实目标是 `A5ED052AB32AE2V`，当前原理图输入不能直接作为 A5ED 方案闭环对象。它只能作为“旧 KU040 + 新 A5EC 方案草图/中间版本”的审核输入，或需要先修正器件库 value / 原理图实例为 A5ED 后再冻结。

## 决策层

这不是小命名问题。`A5EC` 与 `A5ED` 的最大差异是 HPS：当前输入中的 `A5EC052A B32A` 没有 HPS，而用户目标 `A5ED052AB32AE2V` 是带 HPS 的 FPGA SoC。若按当前输入继续设计，控制 MCU 替代、boot、固件升级、复位架构等判断都会偏离目标方案。

下一步必须先确认：当前原理图里的 `A5EC052A B32A` 是临时库名/占位，还是实际选型写错。
