# DF108 / A38 Agilex 5 Revision Index

本页是 `rev-20260506-df108-ku040-to-a5ed052ab32ae2v` 的远端审核入口。它只做导航和状态翻译，不替代 CAD 原理图、Quartus 工程、Pin Planner/Fitter 报告或正式 sign-off。

## Current State

| 主题 | 当前状态 | 审核含义 |
|---|---|---|
| 原理图改版 | `TBD-evidence` | 当前是 KU040 -> Agilex 5 的改版工作区，不能当作发板批准或正式闭环。 |
| LPDDR5 / LPDDR5X | `selected-not-frozen` | Micron `MT62F1G32D2DS-020 WT:D` 可作为主验证候选，但 BOM、pin list、footprint 和 PCB constraints 不能冻结。 |
| GPIO 低速资源 | `TBD-evidence` | 数量口径显示 `205` 需求对 `256` 可统计资源，理论余量 `51`；电压域、bank 粒度和工具链未闭环。 |
| 解码板 168 路 VDDIO | `blocked` / `TBD-evidence` | 若每路都必须支持 `1.2 V` 到 `1.8 V` 可调，必须先确认 3B right、HVIO bank 粒度和 Pin Planner/Fitter。 |
| Formal freeze / sign-off | not reached | 本 revision 目前没有声明 LPDDR5、GPIO、原理图或发板已 sign-off。 |

## Fast Links

| 入口 | 文件 | 用途 |
|---|---|---|
| 当前有效报告 | [04_final_reports/CURRENT.md](04_final_reports/CURRENT.md) | 先看本轮审核口径，避免把 raw fail 误读为已确认设计错误。 |
| GPIO Excel | [02_design_evidence/a38_a5ec052a_b32_low_speed_gpio_resource_assessment_20260512.xlsx](02_design_evidence/a38_a5ec052a_b32_low_speed_gpio_resource_assessment_20260512.xlsx) | 低速 GPIO 需求、资源和分配方案的原始表格证据。 |
| GPIO Markdown 摘要 | [02_design_evidence/a38_a5ec052a_b32_low_speed_gpio_resource_assessment_20260512.md](02_design_evidence/a38_a5ec052a_b32_low_speed_gpio_resource_assessment_20260512.md) | GitHub 上可直接预览的 GPIO 技术层和决策层摘要。 |
| LPDDR5 选型决策 | [05_decisions/20260508-lpddr5-selection.md](05_decisions/20260508-lpddr5-selection.md) | 当前 primary / rejected / watchlist 结论和 freeze blockers。 |
| LPDDR5 selection map | [05_decisions/20260508-lpddr5-selection-map.md](05_decisions/20260508-lpddr5-selection-map.md) | 证据来源、候选漏斗、补证渠道和工具验证路径。 |
| Design evidence | [02_design_evidence/](02_design_evidence/) | 设计方向、资源矩阵、架构图和预检查证据。 |
| Review run index | [03_review_runs/RUN_INDEX.md](03_review_runs/RUN_INDEX.md) | 新旧 run 的索引和防误读入口。 |
| Handoff package | [06_llm_handoff/00_README_FOR_LLM.md](06_llm_handoff/00_README_FOR_LLM.md) | 给其它 LLM 或远端审核者的上下文包入口。 |
| Open questions | [06_llm_handoff/03_open_questions.md](06_llm_handoff/03_open_questions.md) | 仍未闭环的问题、风险和证据缺口。 |

## Status Vocabulary

| 状态 | 使用边界 |
|---|---|
| `selected-not-frozen` | 已选择为工程验证方向，但缺少进入正式冻结所需的 owner signoff、供应商证据、工具链证据或硬件实现证据。 |
| `blocked` | 某个门禁已知缺少必要决策或证据，在补齐前不能进入 freeze。 |
| `TBD-evidence` | 结论方向可以继续调查或画占位，但必须补 Quartus / Pin Planner / Fitter / datasheet / supplier / project signoff 证据。 |
| formal freeze / sign-off | 只有在项目 owner、硬件、逻辑、采购和必要工具链证据全部回写后才可使用；当前 revision 没有达到该状态。 |

## Technical Layer

给硬件审核工程师的最小事实包：

| 主题 | 事实 | 待确认 / 风险 |
|---|---|---|
| Target | Intended target is `A5ED052AB32AE2V`; current schematic placeholder includes `A5EC052A B32A`. | A5EC/A5ED naming, ordering code, package mapping and official pinout still need last-mile evidence. |
| High-speed allocation | Current GPIO assessment assumes LPDDR5/MIPI are already assigned in HSIO, and QSFP high-speed side is already assigned in GTS. | Do not reuse GTS as ordinary low-speed GPIO. |
| Low-speed GPIO demand | Ordinary low-speed GPIO total demand is `205`: decoder board `168` plus 3.3 V control GPIO `37`. | Requirement semantics for decoder board `1.2 V` to `1.8 V` VDDIO remain the key risk. |
| Counted resources | A5E counted low-speed GPIO resources total `256`: HVIO `120`, HSIO 2A `26`, HSIO 2B/3A `24`, HSIO 3B right `48`, HSIO 3B left `38`, GTS `0`. | Pin-level surplus `51` is not voltage-domain closure and does not include bank-granularity loss. |
| 3.3 V GPIO | 3.3 V GPIO should preferentially use HVIO. | HVIO bank VCCIO grouping must be checked, not just aggregate pin count. |
| LPDDR5 | Micron `MT62F1G32D2DS-020 WT:D` is the current primary validation candidate. | Capacity change, supplier lifecycle/grade/commercial terms, derating guidance, Quartus EMIF, Pin Planner, Fitter, package/SI/PI remain open. |

## Decision Layer

给项目经理和跨部门的当前读法：

| 风险 | 业务含义 | Owner | 下一步 |
|---|---|---|---|
| GPIO 数量够但电压域未闭环 | 可以继续推进资源草案；不能承诺 GPIO 已可发板。若解码板必须支持全范围 VADJ，可能带来原理图、layout、Pin Planner 返工。 | 需求 / 架构 + 硬件 + 逻辑 | 先冻结解码板 VDDIO 语义，再跑 Pin Planner/Fitter 粗分配。 |
| LPDDR5 primary 未冻结 | 采购可以继续问价和拿证据；硬件可以做预研，但不能锁 BOM、footprint 或 pin list。 | Project owner + procurement + hardware + logic | 先完成容量变更决策、供应商证据和完整资源共存验证。 |
| A5ED exact target 未闭环 | 当前工作区可以服务 Rev1 占位和风险识别；不能作为正式 A5ED 发布基线。 | Project owner + hardware | 补官方 ordering code、pinout/package、reference design 和工具链证据。 |

## Do Not Overstate

- 不要把 `205` 对 `256` 的数量余量写成电压域已闭环。
- 不要宣称 LPDDR5、GPIO、原理图或发板已 sign-off。
- 不要把 `selected-not-frozen` 升级成 formal freeze。
- 不要把 `TBD-evidence` 的工具链或供应商缺口写成已经通过。
