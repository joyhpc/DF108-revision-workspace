# Key Facts

## Task Facts

| Field | Value |
|---|---|
| project_id | `DF108` |
| revision_id | `rev-20260506-df108-ku040-to-a5ed052ab32ae2v` |
| workflow | `main_controller_migration` |
| intended migration | `KU040 -> Agilex 5` |
| intended target chip | `A5ED052AB32AE2V` |
| external/peripheral preservation | 8 FAKRA, POC, DPS, enclosure, optical-port physical form factor |

## Input Facts

| Field | Value |
|---|---|
| Drive file name | `A38_MAIN_V1_2_A1_3 with Agile package allegro.zip` |
| Drive file id | `1EBJmVgv9b4UBjW6RR6rnBEblP9ZyhRI8` |
| downloaded zip sha256 | `d6509ce856b05ff043cd1b1d47d436fa32a987b4185eb59b1c83ca8092d4b4a8` |
| extracted BOM | `A38_MAIN_V1_2_A1_3.BOM` |
| extracted PST files | `pstchip.log`, `pstxnet.log`, `pstxprt.log` |
| normalized PST files | `pstchip.dat`, `pstxnet.dat`, `pstxprt.dat` |
| normalization type | filename compatibility only; no netlist content rewrite |

## Intake Facts

| Field | Value |
|---|---|
| intake status | pass |
| categories | `bom=1`, `netlist=3` |
| content hash | `0a3121174ab594009795e44b25eec9c00ba0d8235062ac3bd36ba32aea49209a` |
| snapshot path | `01_inputs/snapshot/snapshots/DF108/task-20260506-df108-ku040-a5ed052ab32ae2v-intake/` |

## Schematic/BOM Facts

| Fact | Evidence |
|---|---|
| `U9` is `A5EC052A B32A` | BOM item 126 |
| `U14` is `XCKU040-2FFVA1156I` | BOM item 129 |
| PST chip data contains old KU040 value | `VALUE='XCKU040-2FFVA1156I'` |
| PST chip data contains new Agilex value as A5EC | `PART_NAME='A5EC052A B32A'`, `VALUE='A5EC052A B32A'` |

## User Correction Facts

| Fact | Value |
|---|---|
| old schematic baseline | user states it should be treated as correct for this task |
| current Agilex state | new chip package/scheme added as placeholder |
| C/D package handling | package unified at this stage |
| name mismatch | to be corrected later |
| judgment impact | do not convert raw review errors directly into confirmed schematic design errors |

## Opendatasheet Facts

| Field | A5EC052A_B32A | A5ED052A_B32A |
|---|---|---|
| device role | FPGA | FPGA SoC |
| HPS | none | quad |
| transceiver | true | true |
| crypto | false | true |
| opendatasheet export | available | available |

## Initial Review Facts

| Field | Value |
|---|---|
| review status | fail |
| engines | 6 |
| errors | 40 |
| warnings | 197 |
| infos | 275 |
| execution_errors | 1 |
| skipped | 2 |
| tool issue | `DiffPairCheck` missing `pair_name` attribute |

## Most Important Interpretation

The raw review result must be interpreted through the revision precheck judgment mode:

| Interpreted Field | Value |
|---|---:|
| confirmed design errors | 0 |
| tool issues | 1 |
| boundary / missing-evidence items | 47 |
| package / symbol integration TODOs | 9 |
| warnings requiring triage | 197 |

The current schematic input cannot yet be treated as formal `A5ED052AB32AE2V` sign-off evidence. However, because the user clarified the current state is a package/scheme placeholder on a correct old schematic, the `A5EC` vs `A5ED` naming difference should be treated as a naming consistency TODO until official pinout/power/order-code evidence proves a real incompatibility.

## 2026-05-07 Design Direction Facts

| Field | Value |
|---|---|
| MIPI topology | decoder board MIPI D-PHY -> connector -> direct routing -> `A5EC052A B32A` MIPI-capable HSIO bank |
| MIPI board-level switches/buffers | remove HS/LP switching circuit and buffer |
| MIPI speed boundary | E-Series Group A: up to `3.5 Gbps/lane` for short/standard channel; use `2.5 Gbps/lane` for long/lossy channel until SI evidence proves otherwise |
| memory change | DDR4 -> LPDDR5 |
| LPDDR5 design target | `3,733 Mbps/pin` for current `A5EC052A B32A` / E-Series Group A interpretation |
| LPDDR5 raw bandwidth | `x16` about `7.46 GB/s`; `x32` about `14.93 GB/s` |
| LPDDR5 caution | higher EMIF parameter choices are not automatically valid for the exact device/package/speed grade |
| input power | migrate mature LM5060 front-end circuit |
| LM5060 caution | reuse topology, but re-check UV/OV, current limit, MOSFET SOA, inrush, downstream capacitance, and PG/FLT sequencing |
| next artifact | `A5EC052A B32A resource allocation matrix` covering MIPI, LPDDR5 EMIF, power, clock/reset, and final naming |

Reference files used for this update came from the user-provided Drive folder `1LBmcH09JFtY-A9iW-TYNtksNjdZ7o8wS`, including Agilex 5 Device Overview, Device Data Sheet, EMIF IP User Guide, General-Purpose IO User Guide, MIPI D-PHY IP User Guide, and `altera-pbc-b32a-a5e.xlsx`.
