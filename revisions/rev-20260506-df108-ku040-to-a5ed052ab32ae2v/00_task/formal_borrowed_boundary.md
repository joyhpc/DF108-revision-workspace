# Formal / Borrowed Boundary

本文件用于区分正式对象和借用验证对象。借用对象只能作为证据或风险输入，
不能在 `sch-review` 或 `prj` 工作区内直接升级为项目正式结论。

## 0. 任务上下文

| 字段 | 内容 |
|---|---|
| project_id | DF108 |
| revision_id | rev-20260506-df108-ku040-to-a5ed052ab32ae2v |
| workflow_id | main_controller_migration |
| source_request | DF108 原理图改版任务：在既有 DF108 原理图基础上新增主芯片方案，KU040 -> Agilex 5 A5ED052AB32AE2V，保持 8 路 FAKRA、POC、DPS、机壳和光口物理形态不变；当前原理图位于 Google Drive 文件夹 https://drive.google.com/drive/folders/1FLudfopFvV_cuZyTfbZZf27EL1GUJj6m?dmr=1&ec=wgc-drive-%5Bmodule%5D-goto |

## 1. 对象边界表

| 对象 | repo / path | revision / version | owner | formal or borrowed | 用途 | 状态 |
|---|---|---|---|---|---|---|
| 正式需求基线 |  |  |  | formal / missing | 改版约束 | open |
| 当前原理图导出 | `https://drive.google.com/drive/folders/1FLudfopFvV_cuZyTfbZZf27EL1GUJj6m?dmr=1&ec=wgc-drive-%5Bmodule%5D-goto` | Drive folder, not materialized | user provided | formal candidate | 审核输入 | blocked: missing local_path |
| 旧版原理图 / BOM |  |  |  | formal / borrowed | 差异对照 | open |
| requirements.yaml |  |  |  | formal / missing | 约束输入 | open |
| system.yaml |  |  |  | formal / missing | 多板 link 输入 | open |
| 供应商 reference design |  |  |  | borrowed | 参考证据 | open |
| A5ED052A/B32A opendatasheet export | `/home/ubuntu/knowledge/opendatasheet/data/sch_review_export/A5ED052A_B32A.json` | sha256 `65393d2fc8fcf03a6066b21f299e55e35e284068266f6c18c5f33f2f996f51b7` | opendatasheet | borrowed | 器件 pin/bank/rail/capability 证据 | usable for draft evidence |
| A5EC052A/B32A opendatasheet export | `/home/ubuntu/knowledge/opendatasheet/data/sch_review_export/A5EC052A_B32A.json` | sha256 `07dd0fbd198307e3cbc629d0313bdb7cf219c5a1f9be8f9e97f4f03272a616db` | opendatasheet | borrowed | 当前原理图 `U9=A5EC052A B32A` 证据对照 | usable for mismatch triage |
| A5ED052A/B32A pinout parse | `/home/ubuntu/knowledge/opendatasheet/data/extracted_v2/fpga/pinout/intel_agilex5_a5ed052a_b32a.json` | sha256 `1733593812ede195b0a1bd59228b7d6288b69b82f29809456b9c354e6fd836be` | opendatasheet | borrowed | pinout 解析源 | usable for draft evidence |
| A57 A5ED052A 深度评估 | `/home/ubuntu/hardware-projects/A57-docs/01_需求阶段_Requirements/00_项目级需求_Project_Level/A5ED052A_B32A_单芯片替代_KU3P_STM32_深度评估_2026-04-01.md` | sha256 `8a56c7b1b918e2643973fc1671d3793d41b0c5e1978037c2691486bfb46851d0` | A57-docs | borrowed | 历史方案参考 | usable as reference only |
| A57 A5ED052A 可行性总览 | `/home/ubuntu/hardware-projects/A57-docs/01_需求阶段_Requirements/00_项目级需求_Project_Level/A5ED052A_B32A_CAMRX_DCURX_可行性总览_2026-04-01.md` | sha256 `cddcae008d3d9a1b6cf0c3629e79d7c4037839642113eb6f15f7e49ce54b2c0b` | A57-docs | borrowed | 历史方案参考 | usable as reference only |

## 2. 生效规则

- `formal` 对象的有效版本只能由项目 repo 维护。
- `borrowed` 对象必须记录来源 repo/path、revision、owner 和借用目的。
- `sch-review` 可以引用借用证据形成风险，但不能宣布正式关闭。
- 若缺少正式基线，本次报告必须把它列为 `missing_evidence`。
