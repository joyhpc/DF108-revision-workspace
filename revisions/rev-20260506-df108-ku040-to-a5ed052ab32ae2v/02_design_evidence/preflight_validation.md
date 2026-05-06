# Preflight Validation

本文件记录本次真实应用的第一步验证结果。范围限定为 workflow、workspace、输入源和器件证据，不做原理图风险结论。

## 技术层

| 检查项 | 结果 | 证据 |
|---|---|---|
| revision workflow 识别 | pass | `main_controller_migration`, confidence `0.95` |
| revision workspace 创建 | pass | `/home/ubuntu/hardware-projects/prj/DF108/revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v` |
| task JSON 生成 | pass | `/home/ubuntu/workspace/agents/sch-review/data/inbox/task-20260506-df108-ku040-a5ed052ab32ae2v-start.json` |
| 默认检查集 | pass | `power_tree`, `netlist`, `bom`, `constraints`, `emc` |
| Google Drive 可达性 | pass | HTTP 200，可打开 Drive HTML 页面，并解析到 file id `1EBJmVgv9b4UBjW6RR6rnBEblP9ZyhRI8` |
| Google Drive 输入 materialized | pass | 已下载 `A38_MAIN_V1_2_A1_3_with_Agile_package_allegro.zip` |
| 输入快照 | pass | `bom=1`, `netlist=3`, content hash `0a3121174ab594009795e44b25eec9c00ba0d8235062ac3bd36ba32aea49209a` |
| 初始工具审核 | preliminary fail | 6 个引擎，40 errors, 197 warnings, 275 infos, 1 execution_error |
| opendatasheet A5ED052A/B32A | pass | `/home/ubuntu/knowledge/opendatasheet/data/sch_review_export/A5ED052A_B32A.json` |
| 原理图新增芯片与用户目标一致性 | fail | BOM/网表中 `U9=A5EC052A B32A`，不是 `A5ED052AB32AE2V` |
| 完整 A5ED052AB32AE2V 订购码 | partial | 当前只映射到 `A5ED052A_B32A`，`E2V` 尾缀待官方资料复核 |

## 决策层

当前工具流已经证明：这类“DF108 主芯片替换 / KU040 -> Agilex 5”任务会自动进入主控替换型改版工作流，且中间产物没有写入 `sch-review` 工具仓，而是进入独立 `prj` 工作区。输入已从 Google Drive materialize，并完成 intake 快照。

当前不能作为 A5ED 方案进入正式闭环，原因是原理图/BOM 中新增器件为 `A5EC052A B32A`，与用户目标 `A5ED052AB32AE2V` 不一致。这个差异会直接影响 HPS、boot、控制 MCU 替代和配置链路判断。

## 下一步建议

1. 先确认 `U9=A5EC052A B32A` 是临时占位还是实际选型错误。
2. 若目标确认为 `A5ED052AB32AE2V`，先修正原理图库 value / part mapping，再重新导出 BOM 和 PST 网表。
3. 修复 `board_review` 的 `DiffPairCheck.pair_name` 工具错误后重跑，避免把工具异常混入设计风险。
4. 上传 reference design 后，登记到 `01_inputs/raw/reference_designs/`，再进入 `MCM-G4` 差异 gate。
