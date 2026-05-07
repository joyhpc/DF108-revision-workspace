# LLM Navigation

把 GitHub 链接交给其它 LLM 时，优先让它从这个文件开始读。

这个文件不是证据正文，而是导航层。它的目标是让没有本地上下文、没有 `sch-review` 工具、没有项目历史的 LLM，快速理解应该读哪些文件、按什么顺序读、哪些结论不能越界。

## 任务一句话

DF108 当前是一个原理图改版验证任务：在既有 DF108 / A38 主控原理图基础上，识别并验证“KU040 -> Agilex 5 A5ED052AB32AE2V”主芯片替换任务的输入、边界、证据和初步风险。

当前状态不是原理图 sign-off、不是发板批准、也不是正式项目闭环。

## 最新判断修正

用户已补充说明：当前输入是在一张正确的既有原理图上新增新芯片封装/方案占位；C 型和 D 型封装统一，当前名称不一致后续会修订。

因此，初始审核中的 raw `status=fail` / `errors=40` 不应被直接解释为“原理图有 40 个设计错误”。本轮应按“主控替换型改版预审 / 封装占位阶段”理解：

- 已确认设计错误：0
- 工具问题：1
- 边界/缺证项：47
- 封装/符号集成待办：9
- warnings 待后续 triage：197

优先读取本轮判断解释：

- [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/04_final_reports/CURRENT.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/04_final_reports/CURRENT.md)
- [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/03_review_runs/RUN_INDEX.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/03_review_runs/RUN_INDEX.md)
- [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/03_review_runs/run-20260507-judgment-v2/judgment_interpretation.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/03_review_runs/run-20260507-judgment-v2/judgment_interpretation.md)
- [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/judgment_mode_correction_20260506.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/judgment_mode_correction_20260506.md)

## 最新设计方向

2026-05-07 用户新增设计输入：

- MIPI 去掉 HS/LP 切换开关和 buffer，由解码板经连接器后直连 `A5EC052A B32A` 的 MIPI-capable HSIO bank。
- DDR4 改为 LPDDR5。
- 电源入口使用成熟 LM5060 方案迁移。

当前设计建议：

- MIPI 直连方案成立，但必须按 Agilex 5 MIPI D-PHY IP、HSIO bank、RZQ/refclk、lane placement 规则处理，不能按普通差分 IO 处理。
- 对当前 `A5EC052A B32A` / Agilex 5 E-Series Group A 口径，LPDDR5 设计上限按 `3,733 Mbps/pin`，`x32` raw bandwidth 约 `14.93 GB/s`。
- LM5060 入口电路可结构复用，但要按新 Agilex 5 + LPDDR5 电源树重新核算 current limit、inrush、MOSFET SOA 和 PG/FLT sequencing。

优先读取：

- [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/current_design_direction_20260507.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/current_design_direction_20260507.md)
- [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/06_llm_handoff/04_current_design_direction.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/06_llm_handoff/04_current_design_direction.md)

## 最小阅读路径

如果只能读取少量文件，按这个顺序读：

1. [`README.md`](README.md)
2. [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/04_final_reports/CURRENT.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/04_final_reports/CURRENT.md)
3. [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/03_review_runs/RUN_INDEX.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/03_review_runs/RUN_INDEX.md)
4. [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/03_review_runs/run-20260507-judgment-v2/judgment_interpretation.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/03_review_runs/run-20260507-judgment-v2/judgment_interpretation.md)
5. [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/current_design_direction_20260507.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/current_design_direction_20260507.md)
6. [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/architecture_diagrams/old_ku040_architecture.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/architecture_diagrams/old_ku040_architecture.md)
7. [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/architecture_diagrams/new_agilex_placeholder_architecture.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/architecture_diagrams/new_agilex_placeholder_architecture.md)
8. [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/06_llm_handoff/00_README_FOR_LLM.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/06_llm_handoff/00_README_FOR_LLM.md)
9. [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/06_llm_handoff/01_design_context.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/06_llm_handoff/01_design_context.md)
10. [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/06_llm_handoff/02_key_facts.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/06_llm_handoff/02_key_facts.md)
11. [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/06_llm_handoff/03_open_questions.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/06_llm_handoff/03_open_questions.md)
12. [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/06_llm_handoff/04_current_design_direction.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/06_llm_handoff/04_current_design_direction.md)

这组文件足够让 LLM 建立任务上下文，并知道哪些事实已确认、哪些仍是待确认问题。

## 深入证据路径

当需要查证或做工程判断时，再读取这些文件：

- [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/00_task/revision_brief.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/00_task/revision_brief.md): 改版任务卡
- [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/source_vs_target_chip_check.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/source_vs_target_chip_check.md): 源芯片与目标芯片核对
- [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/current_design_direction_20260507.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/current_design_direction_20260507.md): MIPI 直连、LPDDR5、LM5060 迁移方向
- [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/preflight_validation.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/preflight_validation.md): 输入预检查
- [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/04_final_reports/step1_application_validation_summary.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/04_final_reports/step1_application_validation_summary.md): 本轮应用验证摘要
- [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/04_final_reports/schematic_revision_review.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/04_final_reports/schematic_revision_review.md): 原理图改版审核报告
- [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/architecture_diagrams/architecture_diagram_generation.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/architecture_diagrams/architecture_diagram_generation.md): 架构图生成方式说明
- [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/03_review_runs/run-task-20260506-df108-ku040-a5ed052ab32ae2v-intake/review_results.json`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/03_review_runs/run-task-20260506-df108-ku040-a5ed052ab32ae2v-intake/review_results.json): 结构化审核结果
- [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/06_llm_handoff/evidence_refs.json`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/06_llm_handoff/evidence_refs.json): 证据索引

## 原始输入路径

只有在 LLM 需要查具体网络、器件、BOM 行或原始导出证据时，才读取这些文件：

- [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/01_inputs/raw/normalized_for_intake/A38_MAIN_V1_2_A1_3.BOM`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/01_inputs/raw/normalized_for_intake/A38_MAIN_V1_2_A1_3.BOM)
- [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/01_inputs/raw/normalized_for_intake/pstchip.dat`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/01_inputs/raw/normalized_for_intake/pstchip.dat)
- [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/01_inputs/raw/normalized_for_intake/pstxnet.dat`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/01_inputs/raw/normalized_for_intake/pstxnet.dat)
- [`revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/01_inputs/raw/normalized_for_intake/pstxprt.dat`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/01_inputs/raw/normalized_for_intake/pstxprt.dat)

不要把这些原始 PST 文件作为 LLM 的第一输入。它们适合证据追溯，不适合作为任务理解入口。

## 当前关键边界

- 当前上传包显示出既有 `XCKU040-FFVA1156` 设计证据。
- `A5ED052AB32AE2V` 相关信息目前来自局部 opendatasheet 和任务描述，仍需后续参考设计、pinout、power guide、official datasheet 做 last-mile 校核。
- `A5EC` / `A5ED` 当前先按名称占位处理，不自动当成架构错误；正式输出前仍需修订名称和官方资料证据。
- 本仓库中的 `sch-review` 输出是审核证据，不等同于正式项目结论。
- 借用验证对象、工具运行输出、开放问题必须和正式设计冻结结论分开处理。
- `03_review_runs/*/runtime_repo/` 是本机运行沙箱，不进入 GitHub，也不应作为正式证据路径。

## 建议给其它 LLM 的提示词

可以把下面这段和本仓库链接一起给其它 LLM：

```text
请先阅读仓库根目录的 LLM_NAVIGATION.md，然后按其中“最小阅读路径”理解 DF108 原理图改版任务。

你的目标不是宣布设计已闭环，而是基于仓库中的证据，输出：
1. 已确认事实
2. 待确认问题
3. 主要工程风险
4. 下一步需要补充的输入文件
5. 技术层结论和决策层结论

请明确区分：原始证据、工具推导、任务假设、开放问题、正式结论。
```

## 期望输出格式

其它 LLM 如果参与评审，输出应分两层：

- 技术层：给审核工程师，写清证据来源、网络/器件/文件路径、风险机制和需要补证的点。
- 决策层：给项目经理和跨部门，用交付影响、返工风险、排期风险、采购/资料缺口来表达。

不要只输出“看起来可以”或“建议继续”。这类任务需要证据、边界和下一步动作。
