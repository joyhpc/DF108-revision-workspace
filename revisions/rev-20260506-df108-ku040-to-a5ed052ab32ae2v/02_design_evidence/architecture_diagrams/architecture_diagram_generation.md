# Architecture Diagram Generation Notes

## 生成方式

本轮架构图采用“证据锚点 + 人工结构化 + Mermaid 输出”的方式生成。

它不是从 `pstxnet.dat` 自动布局生成的完整电气连接图。原因是：

- PST 网表适合做 pin/net 级追溯，不适合直接表达项目级系统架构。
- 当前输入是“正确旧图 + 新芯片封装/方案占位”，系统架构需要结合用户补充说明才能正确解释。
- 旧/新架构图的目标是给审核和外部 LLM 建立阅读框架，而不是替代原理图。

## 执行步骤

1. 固化旧报告，避免重跑覆盖旧结论：

```bash
cp 04_final_reports/schematic_revision_review.md \
  04_final_reports/schematic_revision_review__run-task-20260506-df108-ku040-a5ed052ab32ae2v-intake.md
```

2. 从旧 workspace task 生成新的 append-only task：

```bash
jq '... set task_id=task-20260507-df108-judgment-v2 ...' \
  /home/ubuntu/workspace/agents/sch-review/data/inbox/task-20260506-df108-ku040-a5ed052ab32ae2v-intake.json \
  > /home/ubuntu/workspace/agents/sch-review/data/inbox/task-20260507-df108-judgment-v2.json
```

3. 重跑 workspace review：

```bash
python3 -m src.cli --repo-root /home/ubuntu/hardware-projects/sch-review \
  workspace run \
  /home/ubuntu/workspace/agents/sch-review/data/inbox/task-20260507-df108-judgment-v2.json \
  -f json
```

4. 用 BOM/PST 快速提取架构锚点：

```bash
rg -n "XCKU|A5EC|A5ED|QSFP|DDR|FLASH|MCU" \
  01_inputs/raw/normalized_for_intake/A38_MAIN_V1_2_A1_3.BOM

rg -n "XCKU|A5EC|A5ED|QSFP|DDR|FLASH|MCU" \
  01_inputs/raw/normalized_for_intake/pstchip.dat
```

5. 根据证据锚点和用户补充说明，人工生成 Mermaid 图：

- `old_ku040_architecture.md`
- `new_agilex_placeholder_architecture.md`
- `target_a5ed_migration_architecture.md`

## 证据与人工判断边界

| 内容 | 来源 | 可信用途 |
|---|---|---|
| `U14 = XCKU040-2FFVA1156I` | BOM / PST | 旧主控事实 |
| `U9 = A5EC052A B32A` | BOM / PST | 当前新增封装/方案占位事实 |
| `A5ED052AB32AE2V` | 用户任务描述 | 目标命名 / 目标方案 |
| C/D 封装统一、名称后续修订 | 用户补充说明 | 判断模式修正 |
| 8 路 FAKRA、POC、DPS、机壳、光口物理形态保持 | 用户任务描述 | 外设保持边界 |
| DDR / Flash / MCU / QSFP | BOM / PST grep | 架构锚点 |

## 注意事项

- Mermaid 图是审核导航和沟通图，不是原理图连接证明。
- 任何线条若要进入 sign-off，必须回到 BOM/PST、原理图、pinout、reference design 或正式 requirements 中找证据。
- 当前图中的 Agilex 5 路径是 placeholder / target intent，不代表已完成电气连接。
