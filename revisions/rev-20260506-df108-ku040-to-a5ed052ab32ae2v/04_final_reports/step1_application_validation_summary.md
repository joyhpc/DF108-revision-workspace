# Step 1 Application Validation Summary

本文件是 DF108 `KU040 -> Agilex 5` 改版任务的第一步实际应用验证摘要。它不是正式原理图 sign-off，也不是发板结论。

## 技术层

| 项 | 结果 |
|---|---|
| workflow route | pass: `main_controller_migration` |
| revision workspace | pass: `/home/ubuntu/hardware-projects/prj/DF108/revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v` |
| Drive file | pass: `A38_MAIN_V1_2_A1_3 with Agile package allegro.zip`, file id `1EBJmVgv9b4UBjW6RR6rnBEblP9ZyhRI8` |
| raw zip sha256 | `d6509ce856b05ff043cd1b1d47d436fa32a987b4185eb59b1c83ca8092d4b4a8` |
| unpacked files | `A38_MAIN_V1_2_A1_3.BOM`, `pstchip.log`, `pstxnet.log`, `pstxprt.log` |
| normalized intake | copied PST `.log` files to `.dat` names under `01_inputs/raw/normalized_for_intake/` |
| intake validation | pass: `bom=1`, `netlist=3` |
| intake content hash | `0a3121174ab594009795e44b25eec9c00ba0d8235062ac3bd36ba32aea49209a` |
| review run | preliminary tool run completed |
| review summary | `errors=40`, `warnings=197`, `infos=275`, `execution_errors=1`, `skipped=2` |
| generated report | `04_final_reports/schematic_revision_review.md` |

### 关键发现

| 发现 | 证据 | 判定 |
|---|---|---|
| 用户目标为 `A5ED052AB32AE2V` | 用户输入 | target |
| 当前 BOM/网表新增器件为 `U9=A5EC052A B32A` | BOM item 126; `pstchip.dat` `PART_NAME='A5EC052A B32A'` | mismatch |
| 当前 BOM/网表仍保留 `U14=XCKU040-2FFVA1156I` | BOM item 129; `pstchip.dat` `VALUE='XCKU040-2FFVA1156I'` | expected if this is dual-scheme draft; must clarify if old KU040 should remain |
| `A5EC052A` 与 `A5ED052A` 架构差异 | opendatasheet exports | `A5EC`: FPGA/no HPS; `A5ED`: FPGA SoC/quad HPS |
| board_review 有工具异常 | `DiffPairCheck` object has no attribute `pair_name` | tool issue;不能当成板级设计缺陷 |

## 决策层

流程验证通过：这类主芯片替换任务已经可以自动进入 revision workflow，输入、快照、运行产物都落在 `prj` 工作区，workspace outbox 只保留响应引用。

当前不能把本次审核当成 `A5ED052AB32AE2V` 方案结论。原因是输入文件里新增的 Agilex 器件实际是 `A5EC052A B32A`，而 `A5EC` 没有 HPS；如果项目目标是用 HPS 替代控制 MCU 或重做 boot/升级链路，那么当前原理图输入和目标方案不一致。

初始工具审核返回 fail，但这一轮只作为预检：其中一项是工具异常，两个检查缺少约束输入，Power Tree 报告也需要结合“旧 KU040 + 新 Agilex 双方案并存”的上下文人工复核。

## 下一步 Gate

1. 先确认 `U9=A5EC052A B32A` 是否为临时占位。如果目标是 `A5ED052AB32AE2V`，应先修正原理图库 value/part mapping 后重新导出。
2. 明确 `U14=XCKU040-2FFVA1156I` 在这版中是否允许保留。如果只是“新增方案”展示，可保留；如果是目标改版原理图，则需要定义旧主控去留边界。
3. 修复 `board_review` 的 `DiffPairCheck.pair_name` 工具异常后重跑，以免工具问题污染风险台账。
4. 补正式 DF108 baseline、requirements/system 约束和 reference design，再进入 MCM-G1 到 MCM-G4。
