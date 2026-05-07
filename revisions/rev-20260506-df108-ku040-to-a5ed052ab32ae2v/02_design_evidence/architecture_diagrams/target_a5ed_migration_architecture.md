# Target Architecture - A5ED052AB32AE2V Migration Intent

本图描述后续正式迁移完成后应验证的目标架构。它是“目标审核框架”，不是当前输入已经完成的原理图事实。

## Diagram

```mermaid
flowchart LR
  subgraph EXT["DF108 外部/结构保持域 - 必须保持"]
    FAKRA["8 路 FAKRA"]
    POC["POC"]
    DPS["DPS"]
    ENC["机壳 / 线束 / 工装"]
    OPT["光口物理形态 / QSFP CON2"]
    VIN["DC24V / 外部电源"]
  end

  subgraph A5["目标主控域"]
    A5ED["Agilex 5 A5ED052AB32AE2V"]
    FABRIC["FPGA Fabric"]
    HPS["HPS 是否启用 - 架构决策"]
    EMIF["EMIF / DDR"]
    GTS["GTS Transceiver / refclk"]
    CFG["Configuration / Reset / Boot"]
    PWR["Agilex 5 Power Tree / Sequencing"]
  end

  subgraph MIG["必须补齐的迁移证据"]
    PIN["官方 pinout / package file"]
    POWER["Power Management User Guide rail 表"]
    REF["Intel reference design delta"]
    IP["Vivado IP -> Quartus IP 等价表"]
    IFKEEP["外设保持矩阵"]
  end

  FAKRA --> IFKEEP
  POC --> IFKEEP
  DPS --> IFKEEP
  ENC --> IFKEEP
  OPT --> IFKEEP
  IFKEEP --> A5ED

  A5ED --- FABRIC
  A5ED --- HPS
  A5ED <--> EMIF
  A5ED <--> GTS
  CFG --> A5ED
  PWR --> A5ED
  GTS <--> OPT

  PIN --> A5ED
  POWER --> PWR
  REF --> A5ED
  IP --> FABRIC
```

## 正式审核条件

- `U9` / BOM / PST / symbol value 已统一为最终目标料号或项目认可的规范名称。
- 官方 pinout、power rail、sequencing、configuration、boot、HPS、transceiver、DDR/EMIF 证据已进入 `02_design_evidence/`。
- 外设保持矩阵证明 8 路 FAKRA、POC、DPS、机壳、光口物理形态未被破坏。
- 再运行完整迁移专项审核，才能把结果用于发板或正式冻结 gate。
