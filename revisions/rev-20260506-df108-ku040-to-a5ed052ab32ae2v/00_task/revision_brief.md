# Schematic Revision Brief

本文件由 `sch-review workspace route` 自动生成，属于过程工作区文档。
它不是正式设计冻结、正式选型或正式关闭结论。

## 0. 任务元数据

| 字段 | 内容 |
|---|---|
| project_id | DF108 |
| revision_id | rev-20260506-df108-ku040-to-a5ed052ab32ae2v |
| task_id | task-20260506-df108-ku040-a5ed052ab32ae2v-start |
| workflow_id | main_controller_migration |
| workflow_name | 主控替换型改版 |
| revision_root | `/home/ubuntu/hardware-projects/prj/DF108/revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v` |
| source_request | DF108 原理图改版任务：在既有 DF108 原理图基础上新增主芯片方案，KU040 -> Agilex 5 A5ED052AB32AE2V，保持 8 路 FAKRA、POC、DPS、机壳和光口物理形态不变；当前原理图位于 Google Drive 文件夹 https://drive.google.com/drive/folders/1FLudfopFvV_cuZyTfbZZf27EL1GUJj6m?dmr=1&ec=wgc-drive-%5Bmodule%5D-goto |

## 1. 自动分类

| 字段 | 内容 |
|---|---|
| matched | True |
| confidence | 0.95 |
| reason | 主控/FPGA 平台迁移类改版，必须进入 Power Tree、配置/复位/boot 和外设保持 gate。 |
| matched_terms | 主芯片, 改版, KU040, Agilex 5, Agilex5 |

## 2. 默认审核范围

power_tree, netlist, bom, constraints, emc

## 3. Gate 清单

| Gate | 名称 | 必需产物 | 状态 |
|---|---|---|---|
| SR-G0 | 输入快照固化 | input_manifest.json, input_hashes.json | open |
| SR-G1 | 改版任务卡 | revision_brief.md, workflow_manifest.json | open |
| SR-G2 | Formal / Borrowed 边界 | formal_borrowed_boundary.md | open |
| SR-G3 | 专项审核 | review_results.json, risk_register.md, evidence_refs.json | open |
| SR-G4 | 决策层报告 | schematic_revision_review.md | open |
| IPR-G1 | 外设域保持矩阵 | interface_preservation_matrix.md | open |
| MCM-G1 | 迁移可行性与目标型号 gate | resource_mapping.md, ip_equivalence.md | open |
| MCM-G2 | Power Tree 重规划 gate | power_tree_draft.yaml | open |
| MCM-G3 | Configuration / Reset / Boot gate | config_reset_boot.md | open |
| MCM-G4 | 官方模型和 reference design 差异 gate | reference_design_delta.md | open |

## 4. 文件管理约束

- `sch-review` 只保存工具、规则、模板、协议和测试。
- 本次改版输入、中间物、运行产物和报告草稿必须写入本 revision_root。
- 正式需求、正式设计决策、正式关闭结论必须回写项目 repo。
- 对缺失证据项输出 `missing_evidence`，不得写“已闭环”。
