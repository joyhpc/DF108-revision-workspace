# Source Inventory

本文件记录本次 DF108 主芯片替换改版的输入来源状态。当前只做输入建档和可达性验证，不形成正式审核结论。

## 1. 当前原理图输入

| 字段 | 内容 |
|---|---|
| 用户描述 | 在既有 DF108 原理图基础上新增主芯片方案 |
| 目标芯片 | `A5ED052AB32AE2V` |
| 迁移关系 | `KU040 -> Agilex 5` |
| 外设保持约束 | 8 路 FAKRA、POC、DPS、机壳、光口物理形态保持 |
| Google Drive folder | `https://drive.google.com/drive/folders/1FLudfopFvV_cuZyTfbZZf27EL1GUJj6m?dmr=1&ec=wgc-drive-%5Bmodule%5D-goto` |
| 可达性 | HTTP 200，可打开 Google Drive HTML 页面 |
| materialized local_path | `/home/ubuntu/hardware-projects/prj/DF108/revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/01_inputs/raw/A38_MAIN_V1_2_A1_3_with_Agile_package_allegro.zip` |
| file id | `1EBJmVgv9b4UBjW6RR6rnBEblP9ZyhRI8` |
| downloaded sha256 | `d6509ce856b05ff043cd1b1d47d436fa32a987b4185eb59b1c83ca8092d4b4a8` |
| intake 状态 | pass after normalization: `bom=1`, `netlist=3` |

## 2. 已发现的本地器件证据

| 对象 | 路径 | sha256 | 用途 | 边界 |
|---|---|---|---|---|
| opendatasheet sch-review export | `/home/ubuntu/knowledge/opendatasheet/data/sch_review_export/A5ED052A_B32A.json` | `65393d2fc8fcf03a6066b21f299e55e35e284068266f6c18c5f33f2f996f51b7` | A5ED052A/B32A 结构化 pin、bank、rail、capability 输入 | borrowed evidence |
| opendatasheet sch-review export for actual schematic value | `/home/ubuntu/knowledge/opendatasheet/data/sch_review_export/A5EC052A_B32A.json` | `07dd0fbd198307e3cbc629d0313bdb7cf219c5a1f9be8f9e97f4f03272a616db` | 当前 BOM/网表中 `U9=A5EC052A B32A` 的器件证据 | borrowed evidence |
| opendatasheet parsed pinout | `/home/ubuntu/knowledge/opendatasheet/data/extracted_v2/fpga/pinout/intel_agilex5_a5ed052a_b32a.json` | `1733593812ede195b0a1bd59228b7d6288b69b82f29809456b9c354e6fd836be` | A5ED052A/B32A pinout 原始解析输入 | borrowed evidence |
| A57 旧评估：深度评估 | `/home/ubuntu/hardware-projects/A57-docs/01_需求阶段_Requirements/00_项目级需求_Project_Level/A5ED052A_B32A_单芯片替代_KU3P_STM32_深度评估_2026-04-01.md` | `8a56c7b1b918e2643973fc1671d3793d41b0c5e1978037c2691486bfb46851d0` | 参考 A5ED052A(B32A) 替代 KU3P/MCU 的历史分析 | borrowed evidence |
| A57 旧评估：可行性总览 | `/home/ubuntu/hardware-projects/A57-docs/01_需求阶段_Requirements/00_项目级需求_Project_Level/A5ED052A_B32A_CAMRX_DCURX_可行性总览_2026-04-01.md` | `cddcae008d3d9a1b6cf0c3629e79d7c4037839642113eb6f15f7e49ce54b2c0b` | 参考 A5ED052A(B32A) 能力边界与风险翻译 | borrowed evidence |

## 3. 当前缺口

| 缺口 | 影响 | 下一步 |
|---|---|---|
| 目标型号与原理图值不一致 | 用户目标是 `A5ED052AB32AE2V`，但当前 BOM/网表中新增芯片为 `U9=A5EC052A B32A`；`A5EC` 是无 HPS FPGA，`A5ED` 是带 quad HPS 的 FPGA SoC | 先确认这是库 value 未更新，还是实际方案不是 A5ED |
| 完整 ordering code `A5ED052AB32AE2V` 未被本地结构化数据完整表达 | 当前 opendatasheet 可覆盖 `A5ED052A_B32A`，不能确认 `E2V` 尾缀对应的速度等级、温度/电压/订购约束 | 后续补 Intel ordering code / datasheet / pinout reference，记录 source revision |
| 旧版 DF108 正式原理图/BOM 未登记 | 无法做差异对照，也无法判定“只新增方案”是否破坏外设域 | 补旧版 DF108 baseline 的 project repo 路径或本地导出 |
| reference design 尚未上传 | 无法做 MCM-G4 reference design 差异 gate | 后续上传后放入 `01_inputs/raw/reference_designs/` 或登记外部路径 |
