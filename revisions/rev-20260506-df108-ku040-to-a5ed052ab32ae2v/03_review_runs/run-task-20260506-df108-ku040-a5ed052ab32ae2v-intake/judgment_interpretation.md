# Revision Judgment Interpretation

| 字段 | 内容 |
|---|---|
| workflow_id | main_controller_migration |
| mode_id | main_controller_migration_precheck |
| mode_name | 主控替换型改版预审判断模式 |
| raw_review_status | fail |
| interpreted_status | evidence_open |

## Headline

原始工具输出有 40 个 ERROR，但在改版预审口径下被解释为 1 个工具问题、47 个边界/缺证项、0 个命名占位项、9 个封装/符号集成待办；当前不能据此判定原理图存在同等数量的设计错误。

## 技术层

raw counts: ERROR 40, WARNING 197, INFO 275, skipped 2。解释后：已确认设计错误 0，工具问题 1，边界/缺证项 47，命名占位项 0，封装/符号集成待办 9。

## 决策层

当前应定义为证据未闭合/判断口径待补强，而不是设计已判错。优先处理 1 个工具问题、47 个边界/缺证项、0 个命名占位项、9 个封装/符号集成待办后复审。

## Counts

| 类型 | 数量 |
|---|---:|
| raw.errors | 40 |
| raw.warnings | 197 |
| raw.infos | 275 |
| raw.execution_errors | 1 |
| raw.skipped | 2 |
| interpreted.confirmed_design_errors | 0 |
| interpreted.tool_issues | 1 |
| interpreted.boundary_or_missing_evidence | 47 |
| interpreted.part_naming_placeholders | 0 |
| interpreted.package_placeholders_or_unintegrated_symbols | 9 |
| interpreted.warnings_requiring_triage | 197 |

## Classes

### informational

- label: 信息项
- priority: P2
- count: 275
- interpretation: 信息项只作为上下文或后续人工判断输入。

| source | rule_id | severity | location | message |
|---|---|---|---|---|
| constraint_checker | CONSTRAINT-NO-INPUT | INFO | /home/ubuntu/hardware-projects/prj/DF108/revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/03_review_runs/run-task-20260506-df108-ku040-a5ed052ab32ae2v-intake/runtime_repo/data/DF108 | 未找到可检查的设计约束，约束冲突检查已跳过。提供 requirements.yaml 或 pipeline_result.design_constraints 后会启用。 |
| emc_checker | EMC-NO-REQ | INFO |  | 未找到 requirements.yaml，跳过 EMC 预评估 |
| rule_engine_v3 | COMP.abnormal_values | INFO |  | R176: 0R 电阻在电源路径上（确认是否为设计意图） |
| rule_engine_v3 | COMP.abnormal_values | INFO |  | R310: 0R 电阻在电源路径上（确认是否为设计意图） |
| rule_engine_v3 | COMP.abnormal_values | INFO |  | R222: 0R 电阻在电源路径上（确认是否为设计意图） |

### warning_triage

- label: 待评估 warning
- priority: P1
- count: 180
- interpretation: warning 需要工程评估，但不应自动升级为阻断性设计错误。

| source | rule_id | severity | location | message |
|---|---|---|---|---|
| rule_engine_v3 | CONN.connected_components | WARNING |  | 电路有 34 个独立分量（可能有断开的子电路） |
| rule_engine_v3 | CONN.device_id_pins | WARNING |  | U14.IO_L12P_T1U_N10_GC_A08_D24_65/H: 地址/ID 引脚未连接 (NC) |
| rule_engine_v3 | CONN.device_id_pins | WARNING |  | U14.IO_T0U_N12_A28_65/HR: 地址/ID 引脚未连接 (NC) |
| rule_engine_v3 | CONN.device_id_pins | WARNING |  | U44.A1+: 地址/ID 引脚未连接 (NC) |
| rule_engine_v3 | CONN.device_id_pins | WARNING |  | U44.A1-: 地址/ID 引脚未连接 (NC) |

### boundary_or_missing_evidence

- label: 边界/缺证项
- priority: P-evidence
- count: 47
- interpretation: 在改版预审阶段先作为边界或缺证处理，需要结合正式基线、接口输入和测试点策略判断。

| source | rule_id | severity | location | message |
|---|---|---|---|---|
| power_tree | PWR-RISK | ERROR | A_DC_PWR | 上游未闭合 / 缺测试点 / 外部依赖: A_DC_PWR (0.0V) |
| power_tree | PWR-RISK | ERROR | A_POC_PWR | 上游未闭合 / 缺测试点 / 外部依赖: A_POC_PWR (0.0V) |
| power_tree | PWR-RISK | ERROR | B_DC_PWR | 上游未闭合 / 缺测试点 / 外部依赖: B_DC_PWR (0.0V) |
| power_tree | PWR-RISK | ERROR | B_POC_PWR | 上游未闭合 / 缺测试点 / 外部依赖: B_POC_PWR (0.0V) |
| power_tree | PWR-RISK | ERROR | C_DC_PWR | 上游未闭合 / 缺测试点 / 外部依赖: C_DC_PWR (0.0V) |

### package_placeholder_or_unintegrated_symbol

- label: 封装/符号尚未集成
- priority: P-evidence
- count: 9
- interpretation: 主控替换预审中，新增芯片封装/符号占位可能尚未完成电源/GND 集成；先作为封装集成待办，不自动判为旧图错误。

| source | rule_id | severity | location | message |
|---|---|---|---|---|
| rule_engine_v3 | PI.ic_grounding | ERROR |  | U9 没有连接到 GND |
| rule_engine_v3 | PI.ic_power_supply | ERROR |  | U122 没有连接到任何电源网络 |
| rule_engine_v3 | PI.ic_power_supply | ERROR |  | U123 没有连接到任何电源网络 |
| rule_engine_v3 | PI.ic_power_supply | ERROR |  | U124 没有连接到任何电源网络 |
| rule_engine_v3 | PI.ic_power_supply | ERROR |  | U125 没有连接到任何电源网络 |

### tool_issue

- label: 工具问题
- priority: P-tool
- count: 1
- interpretation: 工具执行异常或适配问题；需要修工具或缩小检查范围后复跑，不是原理图设计缺陷。

| source | rule_id | severity | location | message |
|---|---|---|---|---|
| board_review | ENGINE-ERROR | ERROR |  | Board review failed: 'DiffPairCheck' object has no attribute 'pair_name' |

## Rules Applied

- 必须区分 raw tool findings、missing evidence、boundary item、confirmed design error。
- 缺少正式基线或约束文件时，输出 missing_evidence；不得直接写成原理图错误。
- 工具执行异常必须归为 tool_issue，不得翻译成设计不可用。
- 外部供电、连接器输入、跨板输入、缺测试点默认归为 boundary_or_missing_evidence，除非已有正式需求证明其违反设计。
- 若输入是“正确旧图 + 新芯片封装/符号占位”，应先判断新增对象、命名一致性和待补证项，不得把旧图既有边界项计为新方案错误。
- C/D 型封装统一或名称临时不一致时，归为 part_naming_placeholder，除非 pinout、HPS、供电或订货码证据已证明电气不兼容。
- 确认设计错误必须有明确证据链：正式需求/目标料号、当前原理图连接、厂商资料或 pinout、违反项。
