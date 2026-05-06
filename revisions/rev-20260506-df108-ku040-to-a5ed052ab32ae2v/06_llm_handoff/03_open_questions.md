# Open Questions

These questions must be answered before this can become a formal A5ED052AB32AE2V schematic review.

## P0: Target Part Identity

1. Is `U9=A5EC052A B32A` a temporary placeholder for `A5ED052AB32AE2V`?
2. If it is a placeholder, should the symbol value, BOM value, and PST netlist be regenerated with `A5ED052AB32AE2V` or an agreed normalized part string?
3. If it is not a placeholder, is the actual design target now `A5EC052A B32A` instead of `A5ED052AB32AE2V`?

Why this matters:

`A5EC` has no HPS. `A5ED` is an FPGA SoC with quad HPS. The answer changes boot, reset, firmware update, MCU replacement, power sequencing, and control-plane architecture.

## P0: KU040 Coexistence

1. Is `U14=XCKU040-2FFVA1156I` intentionally retained as part of a dual-option schematic?
2. Or should the target revision remove/replace KU040 after the Agilex path is selected?
3. If both `U14` and `U9` remain, which one owns each external interface, control signal, clock, reset, DDR, and high-speed lane?

Why this matters:

The review cannot decide whether duplicated power rails, control lines, and high-speed nets are errors or intentional migration scaffolding without this architectural boundary.

## P0: Formal Baseline

1. Where is the official old DF108 schematic/BOM baseline?
2. Which version is the comparison source for “only added the new chip scheme”?
3. Which project repo owns the official requirement baseline and design decision records?

Why this matters:

Without a formal baseline, this run can identify risks and mismatches, but cannot prove peripheral-domain preservation.

## P1: A5ED052AB32AE2V Ordering Code

1. What does the full suffix `E2V` mean in the intended ordering code?
2. Does it alter speed grade, temperature range, voltage grade, package option, lifecycle, or procurement constraints?
3. Which Intel document or distributor ordering record is the authoritative source?

Why this matters:

Local opendatasheet currently provides strong evidence for `A5ED052A_B32A`, but not a full last-mile confirmation of `A5ED052AB32AE2V`.

## P1: Reference Design

1. Which Agilex 5 reference design should be used for power, configuration, reset, HPS boot, DDR/EMIF, and GTS examples?
2. Which parts of the reference design are allowed to be copied?
3. Which parts must be adapted because DF108 preserves existing external interfaces?

## P1: Tooling Issue

1. The initial board review hit `DiffPairCheck` missing `pair_name`. Should this be fixed in `sch-review` before relying on board-level findings?
2. Which subset of the current 40 P0 findings remains after that tool issue is fixed?

## P1: Requirements Inputs

1. Is there a `requirements.yaml` for this DF108 revision?
2. Is there a `system.yaml` or board-to-board interface contract?
3. Are EMC/high-speed constraints available for FAKRA, POC, DPS, optical, GTS, and DDR?

## Suggested Next Prompt For Another LLM

Given the context and facts above, first assess whether the current schematic input is valid for an `A5ED052AB32AE2V` review. Do not assume `A5EC052A B32A` is equivalent to `A5ED052AB32AE2V`. Separate hard facts from assumptions, and propose the minimum set of corrections or confirmations needed before a full schematic review.
