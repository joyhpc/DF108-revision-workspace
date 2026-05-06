# DF108 Revision Workspace

这个仓库用于同步 DF108 原理图改版任务的项目级中间产物，方便在 GitHub 上浏览和协作。

它不是 `sch-review` 工具仓，也不是 DF108 项目的正式发布仓。这里保存的是改版任务工作区产物：输入快照、设计证据、审核运行结果、最终报告和 LLM handoff 包。

## 当前改版

- Revision: [`rev-20260506-df108-ku040-to-a5ed052ab32ae2v`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/)
- 任务类型: 主芯片替换型原理图改版
- 已知目标方案: `A5ED052AB32AE2V`
- 当前输入基线: 基于既有 DF108 / A38 主控原理图包，并加入 Agilex 5 方案相关内容

## 推荐入口

- [`LLM_NAVIGATION.md`](LLM_NAVIGATION.md): 把 GitHub 链接交给其它 LLM 时，优先让它从这里开始读
- [`03_review_runs/.../judgment_interpretation.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/03_review_runs/run-task-20260506-df108-ku040-a5ed052ab32ae2v-intake/judgment_interpretation.md): 本轮 raw 审核结果的改版判断口径解释
- [`02_design_evidence/judgment_mode_correction_20260506.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/judgment_mode_correction_20260506.md): 针对“正确旧图 + 新芯片封装占位”的判断修正
- [`00_task/revision_brief.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/00_task/revision_brief.md): 改版任务卡
- [`02_design_evidence/source_vs_target_chip_check.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/source_vs_target_chip_check.md): 源芯片与目标芯片检查
- [`04_final_reports/step1_application_validation_summary.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/04_final_reports/step1_application_validation_summary.md): 本轮应用验证摘要
- [`04_final_reports/schematic_revision_review.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/04_final_reports/schematic_revision_review.md): 原理图改版审核报告
- [`06_llm_handoff/00_README_FOR_LLM.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/06_llm_handoff/00_README_FOR_LLM.md): 给其它 LLM 平台使用的 handoff 包入口

## 输出边界

- `01_inputs/`: 原始输入、解包文件、normalized_for_intake、输入快照
- `02_design_evidence/`: 设计依据与预检查证据
- `03_review_runs/`: 审核运行记录与结构化输出
- `04_final_reports/`: 面向工程与决策的报告
- `06_llm_handoff/`: 可转交给其它 LLM 的标准化上下文包

`03_review_runs/*/runtime_repo/` 是本机运行审核时生成的临时沙箱，包含绝对路径符号链接，不进入 GitHub。
