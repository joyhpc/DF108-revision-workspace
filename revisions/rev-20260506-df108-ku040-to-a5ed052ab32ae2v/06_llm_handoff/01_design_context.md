# DF108 Schematic Revision Context For External LLM

You are reviewing a hardware schematic revision task for project `DF108`.

The user's intended task is a main-controller replacement style derivative design:

- old main FPGA: Xilinx `XCKU040-2FFVA1156I` / KU040 class;
- intended new main chip: Intel/Altera Agilex 5 `A5ED052AB32AE2V`;
- high-level migration statement: `KU040 -> Agilex 5`;
- board-level constraint: keep the DF108 peripheral domain unchanged, including 8 FAKRA channels, POC, DPS, mechanical enclosure constraints, and optical-port physical form factor.
- 2026-05-08 clarification: target Rev1 should completely delete the old KU040 path; `U14` is not retained as a dual-option controller.
- 2026-05-08 clarification: 168 ordinary decoder-board GPIO signals require adjustable `1.2 V` to `1.8 V` I/O bank support.

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

## User Correction After Initial Review

The user clarified that this input should not be interpreted as a completed Agilex 5 migration schematic waiting for sign-off.

The correct interpretation is:

- the existing DF108 / A38 schematic baseline should be treated as a correct old schematic for this task;
- the current update adds the new Agilex 5 chip package/scheme onto that old schematic;
- C-type and D-type package usage is unified at this stage;
- the current name mismatch will be corrected later.

This means raw tool findings about unintegrated power/GND pins on the newly added package, boundary supplies, missing test points, or `A5EC` / `A5ED` naming should be treated as evidence-gate items, not immediate proof of old-schematic design errors.

## Critical Discovery

The user target says `A5ED052AB32AE2V`.

The current BOM/netlist does not show that exact target part.

The downloaded BOM shows:

- `U9 = A5EC052A B32A`
- `U14 = XCKU040-2FFVA1156I`

The PST chip data also shows:

- old FPGA primitive value: `XCKU040-2FFVA1156I`
- new Agilex primitive value: `A5EC052A B32A`

This was originally treated as the most important issue in the first handoff. After the user correction above, it should be downgraded to a part-name / ordering-code consistency item for the current placeholder stage.

It still must be corrected before formal schematic release, but it should not be used by itself to declare the current old schematic or added package incorrect.

## A5EC vs A5ED

Local opendatasheet exports indicate:

| Item | A5EC052A_B32A | A5ED052A_B32A |
|---|---|---|
| variant code | C | D |
| device role | FPGA | FPGA SoC |
| HPS | none | quad |
| transceiver | true | true |
| crypto | false | true |

Implication for later formal review:

If the final intended design truly depends on Agilex 5 HPS to replace MCU/control functionality, boot handling, firmware update flow, or management-plane responsibilities, then the final schematic, BOM, symbol value, and PST export must all be regenerated with the intended `A5ED052AB32AE2V` naming and checked against official Intel evidence.

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

The remaining P0 items are mostly power-tree and IC supply/grounding findings. The raw input still contains both `U14` KU040 and `U9` Agilex evidence, but the target Rev1 direction has changed: KU040 should be deleted, and old KU040-owned nets must be removed or reassigned rather than treated as intentional dual-scheme coexistence.

Updated judgment-mode interpretation:

- confirmed design errors: `0`
- tool issues: `1`
- boundary / missing-evidence items: `47`
- package / symbol integration TODOs: `9`
- warnings requiring triage: `197`

This updated interpretation is recorded in:

`03_review_runs/run-20260507-judgment-v2/judgment_interpretation.md`

The current valid report pointer is:

`04_final_reports/CURRENT.md`

Architecture diagrams are recorded in:

`02_design_evidence/architecture_diagrams/`

## Recommended Review Focus

First, preserve the corrected task intent:

1. Treat the old DF108 schematic as the correct baseline for this task unless formal evidence says otherwise.
2. Treat `U9=A5EC052A B32A` as a temporary package/value placeholder for the Agilex path.
3. Record that C/D package usage is unified at this stage and final naming will be corrected later.
4. Do not count placeholder-stage power/GND findings as old-schematic design errors.

Only after that should the review proceed to:

- Agilex 5 power-tree rail mapping;
- configuration, reset, boot, and HPS-first or FPGA-first strategy;
- GTS lane/refclk allocation for optical/high-speed links;
- DDR/EMIF planning;
- peripheral domain preservation matrix;
- reference design delta review.

## Current Bottom Line

This input is good enough for workflow validation, intake validation, and early mismatch detection.

It is not yet good enough to declare an `A5ED052AB32AE2V` schematic sign-off result. It is good enough to validate the workflow and capture the next required evidence: final part naming, official pinout/power/reference design, and a later full migration review.
