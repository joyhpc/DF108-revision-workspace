# DF108 Schematic Revision Context For External LLM

You are reviewing a hardware schematic revision task for project `DF108`.

The user's intended task is a main-controller replacement style derivative design:

- old main FPGA: Xilinx `XCKU040-2FFVA1156I` / KU040 class;
- intended new main chip: Intel/Altera Agilex 5 `A5ED052AB32AE2V`;
- high-level migration statement: `KU040 -> Agilex 5`;
- board-level constraint: keep the DF108 peripheral domain unchanged, including 8 FAKRA channels, POC, DPS, mechanical enclosure constraints, and optical-port physical form factor.

This is not simply replacing one IC symbol. It is a main-controller migration task. The review must consider power tree, reset, configuration/boot, high-speed transceiver lanes, DDR/memory interface, HPS usage, control interfaces, and whether the old external interface domain is preserved.

## Current Input Material

The current design input came from a public Google Drive folder. The downloaded file is:

`A38_MAIN_V1_2_A1_3 with Agile package allegro.zip`

The extracted contents were:

- `A38_MAIN_V1_2_A1_3.BOM`
- `pstchip.log`
- `pstxnet.log`
- `pstxprt.log`

For tool intake only, the PST `.log` files were copied to `.dat` names:

- `pstchip.log` -> `pstchip.dat`
- `pstxnet.log` -> `pstxnet.dat`
- `pstxprt.log` -> `pstxprt.dat`

No electrical or netlist content was rewritten during that normalization. It was a filename compatibility step.

The intake snapshot passed with:

- `bom = 1`
- `netlist = 3`
- content hash: `0a3121174ab594009795e44b25eec9c00ba0d8235062ac3bd36ba32aea49209a`

## Critical Discovery

The user target says `A5ED052AB32AE2V`.

The current BOM/netlist does not show that exact target part.

The downloaded BOM shows:

- `U9 = A5EC052A B32A`
- `U14 = XCKU040-2FFVA1156I`

The PST chip data also shows:

- old FPGA primitive value: `XCKU040-2FFVA1156I`
- new Agilex primitive value: `A5EC052A B32A`

This is the most important issue in the current handoff. `A5EC052A` and `A5ED052A` are not equivalent from a system architecture perspective.

## A5EC vs A5ED

Local opendatasheet exports indicate:

| Item | A5EC052A_B32A | A5ED052A_B32A |
|---|---|---|
| variant code | C | D |
| device role | FPGA | FPGA SoC |
| HPS | none | quad |
| transceiver | true | true |
| crypto | false | true |

Implication:

If the intended design truly depends on the Agilex 5 HPS to replace MCU/control functionality, boot handling, firmware update flow, or management-plane responsibilities, then the current schematic input using `A5EC052A B32A` is not aligned with the target `A5ED052AB32AE2V`.

## Initial Tool Review Result

An initial `sch-review` run was performed after intake. It completed, but should be interpreted as preliminary because the target part mismatch is unresolved and some tool/configuration inputs are incomplete.

Summary:

- review status: `fail`
- engines run: 6
- errors: 40
- warnings: 197
- infos: 275
- execution errors: 1
- skipped: 2

Important caveat:

One P0 item is a tool exception: `Board review failed: 'DiffPairCheck' object has no attribute 'pair_name'`. This should be treated as a tool issue, not as a board design defect.

The remaining P0 items are mostly power-tree and IC supply/grounding findings. These need engineering triage in the context of the current schematic being a dual-scheme or intermediate draft with both `U14` KU040 and `U9` Agilex present.

## Recommended Review Focus

First, resolve the target-part identity:

1. Is `U9=A5EC052A B32A` a temporary symbol/value placeholder for `A5ED052AB32AE2V`?
2. Or is the actual schematic using `A5EC052A`, while the task description says `A5ED052AB32AE2V`?
3. Should old `U14=XCKU040-2FFVA1156I` remain in this schematic as a comparison/dual-option page, or should it be removed in the intended revision?

Only after that should the review proceed to:

- Agilex 5 power-tree rail mapping;
- configuration, reset, boot, and HPS-first or FPGA-first strategy;
- GTS lane/refclk allocation for optical/high-speed links;
- DDR/EMIF planning;
- peripheral domain preservation matrix;
- reference design delta review.

## Current Bottom Line

This input is good enough for workflow validation, intake validation, and early mismatch detection.

It is not yet good enough to declare an `A5ED052AB32AE2V` schematic review result, because the actual schematic data currently points to `A5EC052A B32A`.
