# Judgment Mode Correction - 2026-05-06

## 背景

用户补充说明：当前输入不是一张已经完成 KU040 -> Agilex 5 全量迁移并等待 sign-off 的原理图。

当前输入应按以下方式理解：

- 既有 DF108 / A38 原理图基线本身按“已正确的旧图”处理。
- 本轮是在旧图基础上新增 Agilex 5 新芯片封装/方案占位。
- C 型和 D 型封装统一，当前 `A5EC` / `A5ED` 名称差异后续会修订。
- 因此，当前阶段的重点不是判定旧图大量错误，而是验证输入、识别新增封装、记录命名一致性待办、明确后续资料缺口。

## 修正后的判断口径

原始 `sch-review` 工具输出仍作为 raw evidence 保留，但不能直接把 raw `ERROR` 数量等同为已确认原理图设计错误。

本轮 raw 输出解释如下：

| 类型 | 数量 | 解释 |
|---|---:|---|
| raw ERROR | 40 | 工具原始严重度，不等于 40 个设计错误 |
| 已确认设计错误 | 0 | 当前没有足够证据把 raw ERROR 升级为正式设计错误 |
| 工具问题 | 1 | `DiffPairCheck` 缺少 `pair_name`，属于工具适配问题 |
| 边界/缺证项 | 47 | 多为外部供电、上游未闭合、缺测试点、requirements 缺失类边界问题 |
| 封装/符号集成待办 | 9 | 新增芯片/相关符号尚未完成电源和 GND 集成，符合占位阶段特征 |
| warnings 待评估 | 197 | 需要后续按正式需求和目标资料 triage，不自动阻断 |

## 对 `A5EC` / `A5ED` 的处理

原 handoff 中把 `A5EC` / `A5ED` 差异作为最高优先级问题，这个判断需要降级。

修正后：

- 在封装统一且名称后续修订的前提下，`A5EC` / `A5ED` 先归为“料号/命名占位”。
- 它仍然需要在正式输出前修订 BOM、符号值、PST 导出和项目记录。
- 只有当 pinout、HPS、供电 rail、订货码或官方资料证明 C/D 在本设计中存在电气/架构不兼容时，才能升级为架构风险。

## 后续审核应先做什么

1. 固化用户补充说明到任务卡或项目 repo。
2. 标记当前输入阶段为“正确旧图 + 新芯片封装/符号占位”，不是完整迁移 sign-off。
3. 获取目标 `A5ED052AB32AE2V` 官方 pinout、power guide、ordering code、reference design。
4. 重新生成最终名称一致的 BOM / PST / symbol value。
5. 再进入 Agilex 5 power tree、configuration/reset/boot、HPS、transceiver、DDR、外设保持矩阵的专项审核。

## 对外部 LLM 的提示

如果把本仓库交给其它 LLM，请要求它优先读取：

- `LLM_NAVIGATION.md`
- `03_review_runs/.../judgment_interpretation.md`
- 本文件

不要让它只根据 `review_results.json` 里的 raw `status=fail` 和 `errors=40` 得出“原理图有 40 个设计错误”的结论。
