# New Architecture - Current Agilex Package Placeholder

本图描述当前输入的“新架构占位状态”：在既有正确旧图基础上新增 Agilex 5 芯片封装/方案占位，但还不是完整的 KU040 -> A5ED052AB32AE2V 迁移签核图。

## Evidence Anchors

| 对象 | 证据 |
|---|---|
| 旧主控仍在当前输入中 | BOM: `U14 = XCKU040-2FFVA1156I` |
| 新增 Agilex 占位 | BOM/PST: `U9 = A5EC052A B32A` |
| 目标名称 | 用户任务描述：`A5ED052AB32AE2V` |
| C/D 封装关系 | 用户补充：C 型和 D 型封装统一，名称后续再改 |
| 当前判断口径 | `run-20260507-judgment-v2/judgment_interpretation.md` |

## Diagram

```mermaid
flowchart LR
  subgraph EXT["DF108 外部/结构保持域 - 不应改动"]
    FAKRA["8 路 FAKRA"]
    POC["POC"]
    DPS["DPS"]
    ENC["机壳 / 线束 / 工装"]
    OPT["光口物理形态 / QSFP CON2"]
    VIN["DC24V / 外部电源"]
  end

  subgraph OLD["旧主控路径 - 当前仍作为正确基线存在"]
    KU040["U14 XCKU040-2FFVA1156I"]
    OLD_DDR["旧 DDR4"]
    OLD_FLASH["旧 SPI Flash"]
    OLD_CFG["旧配置 / 复位 / 时序"]
  end

  subgraph NEWPH["新增 Agilex 5 封装/方案占位"]
    A5PH["U9 A5EC052A B32A 占位\n目标命名: A5ED052AB32AE2V"]
    A5_PWR["Agilex 5 Power Tree 待重规划"]
    A5_CFG["Active Serial / AVST / HPS boot 待决策"]
    A5_DDR["EMIF / DDR 规划待确认"]
    A5_GTS["GTS / refclk / 光口映射待确认"]
  end

  subgraph TODO["本阶段输出性质"]
    JUDGE["judgment: evidence_open"]
    NAMING["料号/命名一致性待修订"]
    PKG["封装/符号集成待办"]
    REFS["官方 pinout / power guide / reference design 待补"]
  end

  FAKRA --> KU040
  POC --> KU040
  DPS --> KU040
  OPT <--> KU040
  OLD_DDR <--> KU040
  OLD_FLASH --> KU040
  OLD_CFG --> KU040

  FAKRA -.保持边界，后续映射.-> A5PH
  POC -.保持边界，后续映射.-> A5PH
  DPS -.保持边界，后续映射.-> A5PH
  OPT -.GTS/refclk 待规划.-> A5PH
  A5_PWR -.待接入.-> A5PH
  A5_CFG -.待接入.-> A5PH
  A5_DDR -.待接入.-> A5PH
  A5_GTS -.待接入.-> A5PH

  A5PH --> JUDGE
  JUDGE --> NAMING
  JUDGE --> PKG
  JUDGE --> REFS
```

## 解释

- 当前“新架构”不是一个完成迁移的电气闭环架构，而是新增 Agilex 5 封装/方案占位。
- `U9` 的 `A5EC` 名称在当前阶段按占位处理；正式输出前必须改成最终约定的 `A5ED052AB32AE2V` 相关名称，并重新导出 BOM/PST。
- `U14 KU040` 仍在输入中，因此工具看到的旧路径和新占位会共存；审核应先判断边界和占位状态，不应直接按发板前 sign-off 口径判错。
- 本阶段的合理结论是 `evidence_open`：证据和集成待办未闭合。
