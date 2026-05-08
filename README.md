# DF108 Revision Workspace

这个仓库用于同步 DF108 原理图改版任务的项目级中间产物，方便在 GitHub 上浏览和协作。

它不是 `sch-review` 工具仓，也不是 DF108 项目的正式发布仓。这里保存的是改版任务工作区产物：输入快照、设计证据、审核运行结果、最终报告和 LLM handoff 包。

## 当前改版

- Revision: [`rev-20260506-df108-ku040-to-a5ed052ab32ae2v`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/)
- 任务类型: 主芯片替换型原理图改版
- 已知目标方案: `A5ED052AB32AE2V`
- 当前输入基线: 基于既有 DF108 / A38 主控原理图包，并加入 Agilex 5 方案相关内容

## 给原理图设计人员的使用方式

这个仓库可以当作 DF108 第一版原理图改版的设计控制台使用。它不替代 CAD 原理图，也不宣布 sign-off；它负责告诉你当前哪些页可以画、哪些连接只能占位、哪些结论必须等 Quartus / Pin Planner / 官方资料补证。

当前画图状态：

| 分类 | 状态 |
|---|---|
| 已确认 | MIPI 去掉 HS/LP switch 和 buffer，走 decoder board -> connector -> Agilex 5 MIPI-capable HSIO 直连 |
| 已确认 | LPDDR5 按 `2` 组 x32 颗粒推进，每组一个 LPDDR5 hard memory controller |
| 已确认 | 目标第一版需要完全删除 `KU040`，不再作为 dual-option 保留 |
| 已确认 | 解码板过来的 `168` 路普通 GPIO 按 4 组可调 HSIO/VCCIO_PIO bank 占位 |
| 已确认 | 24V 电源入口复用成熟 LM5060 拓扑 |
| 暂定假设 | `A5EC052A B32A` / `A5ED052AB32AE2V` 命名差异先按占位清理项处理 |
| 待补证 | MIPI lane、LPDDR5 EMIF bank/pin、168 GPIO exact bank/pin、RZQ/refclk、电源时序、clock/reset/config |

画图时优先打开：

- [`02_design_evidence/a5ec052a_b32a_resource_allocation_matrix_20260507.csv`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/a5ec052a_b32a_resource_allocation_matrix_20260507.csv): 第一版资源分配矩阵
- [`02_design_evidence/current_design_direction_20260507.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/current_design_direction_20260507.md): 当前设计方向解释
- [`02_design_evidence/ku040_removal_gpio_bank_allocation_20260508.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/ku040_removal_gpio_bank_allocation_20260508.md): KU040 删除与 168 路 GPIO bank 分配判断
- [`06_llm_handoff/03_open_questions.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/06_llm_handoff/03_open_questions.md): 还不能闭合的问题

建议按资源矩阵的 `schematic_page` 列推进原理图：

| schematic_page | 画图用途 |
|---|---|
| `SCH_A5E_SYMBOL` | 主芯片符号分页、A5EC/A5ED 命名占位 |
| `SCH_MIPI_DIRECT` | 解码板连接器到 Agilex 5 HSIO 的 MIPI 直连 |
| `SCH_DECODER_GPIO_VADJ` | 解码板 168 路普通 GPIO，4 组可调 HSIO/VCCIO_PIO bank |
| `SCH_LPDDR5_CTRL0` | 第 1 组 x32 LPDDR5 颗粒和主控资源 |
| `SCH_LPDDR5_CTRL1` | 第 2 组 x32 LPDDR5 颗粒和主控资源 |
| `SCH_POWER_ENTRY` | LM5060 入口保护 / hot-swap 迁移 |
| `SCH_POWER_TREE` | Agilex 5 + 两组 LPDDR5 电源树和 PG/FLT 链 |
| `SCH_CLOCK_RESET_CONFIG` | MIPI refclk、EMIF refclk、reset、config、JTAG |

资源矩阵里的 `status` 是画图门禁：

| status | 对原理图动作的含义 |
|---|---|
| `confirmed` | 可以作为当前事实引用 |
| `assumed_for_rev1` | 可以用于第一版占位绘制，但正式冻结前仍要复核 |
| `pending_quartus` | 等 Quartus IP / resource report，不要凭空定 pin 或资源 |
| `pending_pin_planner` | 等 Pin Planner，不要把 bank / lane 固化 |
| `pending_datasheet` | 等官方 datasheet 或器件资料 |
| `pending_reference_design` | 等参考设计或项目级设计决策 |
| `naming_cleanup` | 先保留占位，正式输出前统一 symbol / BOM / PST 命名 |

每次从 Quartus、Pin Planner、datasheet 或参考设计拿到新证据后，优先回填资源矩阵，再继续画相应页面。这样 GitHub 上能持续看到“当前能画什么、为什么能画、还差什么证据”。

## 推荐入口

- [`LLM_NAVIGATION.md`](LLM_NAVIGATION.md): 把 GitHub 链接交给其它 LLM 时，优先让它从这里开始读
- [`04_final_reports/CURRENT.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/04_final_reports/CURRENT.md): 当前有效报告入口
- [`03_review_runs/RUN_INDEX.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/03_review_runs/RUN_INDEX.md): 新旧 run 索引，避免旧结果误读
- [`03_review_runs/.../judgment_interpretation.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/03_review_runs/run-20260507-judgment-v2/judgment_interpretation.md): 本轮 raw 审核结果的改版判断口径解释
- [`02_design_evidence/current_design_direction_20260507.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/current_design_direction_20260507.md): 当前 MIPI 直连、LPDDR5、LM5060 迁移的设计方向更新
- [`02_design_evidence/architecture_diagrams/`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/architecture_diagrams/): 新旧架构图和生成说明
- [`02_design_evidence/judgment_mode_correction_20260506.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/judgment_mode_correction_20260506.md): 针对“正确旧图 + 新芯片封装占位”的判断修正
- [`00_task/revision_brief.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/00_task/revision_brief.md): 改版任务卡
- [`02_design_evidence/source_vs_target_chip_check.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/02_design_evidence/source_vs_target_chip_check.md): 源芯片与目标芯片检查
- [`04_final_reports/step1_application_validation_summary.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/04_final_reports/step1_application_validation_summary.md): 本轮应用验证摘要
- [`04_final_reports/schematic_revision_review.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/04_final_reports/schematic_revision_review.md): 原理图改版审核报告
- [`06_llm_handoff/00_README_FOR_LLM.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/06_llm_handoff/00_README_FOR_LLM.md): 给其它 LLM 平台使用的 handoff 包入口
- [`06_llm_handoff/04_current_design_direction.md`](revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/06_llm_handoff/04_current_design_direction.md): 给其它 LLM 的当前设计方向摘要

## 输出边界

- `01_inputs/`: 原始输入、解包文件、normalized_for_intake、输入快照
- `02_design_evidence/`: 设计依据与预检查证据
- `03_review_runs/`: 审核运行记录与结构化输出
- `04_final_reports/`: 面向工程与决策的报告
- `06_llm_handoff/`: 可转交给其它 LLM 的标准化上下文包

`03_review_runs/*/runtime_repo/` 是本机运行审核时生成的临时沙箱，包含绝对路径符号链接，不进入 GitHub。
