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

The current schematic input cannot yet be treated as an `A5ED052AB32AE2V` review target. It currently contains `A5EC052A B32A`, and the `A5EC` vs `A5ED` distinction changes whether HPS exists.
