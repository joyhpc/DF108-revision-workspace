# Review Run Index

本索引用于区分同一 revision 下多次审核运行，避免旧 run 与当前有效判断混淆。

## Current Run

| 字段 | 内容 |
|---|---|
| current_run_id | `run-20260507-judgment-v2` |
| task_id | `task-20260507-df108-judgment-v2` |
| status | current |
| reason | 使用 `main_controller_migration_precheck` 判断模式重跑；按“正确旧图 + 新芯片封装/方案占位”解释 raw findings |
| report | [`../04_final_reports/schematic_revision_review__run-20260507-judgment-v2.md`](../04_final_reports/schematic_revision_review__run-20260507-judgment-v2.md) |
| current pointer | [`../04_final_reports/CURRENT.md`](../04_final_reports/CURRENT.md) |
| judgment | [`run-20260507-judgment-v2/judgment_interpretation.md`](run-20260507-judgment-v2/judgment_interpretation.md) |

## Runs

| run_id | task_id | status | interpretation | primary output |
|---|---|---|---|---|
| `run-task-20260506-df108-ku040-a5ed052ab32ae2v-intake` | `task-20260506-df108-ku040-a5ed052ab32ae2v-intake` | superseded | 初始 run；raw `ERROR=40` 的原始结论保留作证据，但不能作为当前判断入口 | [`run-task-20260506-df108-ku040-a5ed052ab32ae2v-intake/review_results.json`](run-task-20260506-df108-ku040-a5ed052ab32ae2v-intake/review_results.json) |
| `run-20260507-judgment-v2` | `task-20260507-df108-judgment-v2` | current | 改版预审判断模式；确认当前为 `evidence_open`，不是 40 个已确认设计错误 | [`run-20260507-judgment-v2/judgment_interpretation.md`](run-20260507-judgment-v2/judgment_interpretation.md) |

## Interpretation Rule

- 旧 run 不删除，用于追溯 raw tool 输出和判断模式演进。
- 当前对外阅读入口必须使用 `current` run。
- 若后续再次重跑，应新增 run 目录并更新本索引，不覆盖旧 run。
