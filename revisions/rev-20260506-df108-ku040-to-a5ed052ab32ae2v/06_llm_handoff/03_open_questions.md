# Open Questions

These questions must be answered before this can become a formal A5ED052AB32AE2V schematic review.

## P1: Target Part Naming

User clarification: `U9=A5EC052A B32A` is currently treated as a temporary placeholder/name mismatch for the Agilex path. C-type and D-type package usage is unified at this stage, and the name will be corrected later.

Remaining questions:

1. What exact normalized string should be used in symbol value, BOM value, and PST export for `A5ED052AB32AE2V`?
2. Which official Intel pinout / ordering-code document confirms that the placeholder package maps correctly to the final D-type target?
3. Does the final design actually use HPS functions, or is HPS presence only a procurement / roadmap option?

Why this still matters:

The naming issue is no longer a P0 design-error claim for the current placeholder input. It still must be closed before formal release because `A5EC` and `A5ED` differ in HPS and ordering semantics.

## P0: KU040 Coexistence

User clarification on 2026-05-08: target Rev1 should completely delete `U14=XCKU040-2FFVA1156I`; it is not intentionally retained as a dual-option schematic path.

Remaining questions:

1. Which old KU040-owned nets are deleted outright versus reassigned to Agilex 5, MCU, decoder board, or preserved external interface logic?
2. Which old KU040 power rails, clocks, resets, configuration devices, DDR4 nets, and test points should be removed from the target schematic?
3. Which historical evidence file is the formal old baseline for proving that all intended peripheral functions survived after KU040 deletion?

Why this matters:

Raw input evidence still contains KU040. For target Rev1, duplicated KU040/Agilex ownership should now be treated as migration work to remove or reassign, not as intentional coexistence.

## P0: Decoder GPIO / Adjustable HSIO Capacity

User clarification on 2026-05-08: 168 ordinary GPIO from the decoder board need adjustable bank voltage from `1.2 V` to `1.8 V`.

Current Rev1 allocation assumption:

1. Split 168 GPIO into four groups of 42.
2. Each group targets one Agilex 5 HSIO / `VCCIO_PIO` sub-bank.
3. Exact banks and pins are pending Quartus / Pin Planner.

Remaining questions:

1. Does the final exact device use A5EC-like HSIO resources or A5ED SoC resources?
2. Can Quartus place `MIPI + 2x LPDDR5 x32 + 168 adjustable GPIO` on the exact B32A device/package/speed grade?
3. What is the decoder board connector pin map and GPIO direction for all 168 signals?
4. Are all 168 GPIO always at the same VADJ voltage, or do they require independently adjustable bank groups?
5. If final A5ED has only four HSIO sub-banks, which architecture change will absorb the resource conflict: fewer GPIO, external expander/CPLD, different FPGA variant, different package, or reduced memory/MIPI resource use?

Why this matters:

Local pinout evidence indicates A5EC052A_B32A has 8 HSIO sub-banks, while A5ED052A_B32A has 4 HSIO sub-banks. 168 GPIO alone requires 4 sub-banks when grouped safely, so A5ED may have no adjustable HSIO left for MIPI and LPDDR5.

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

## P1: MIPI Direct Connection Closure

1. For each MIPI path, what is the decoder source, connector pin map, lane count, lane rate, clock lane, and target A5EC HSIO bank/lane?
2. Does the decoder board output a standard MIPI D-PHY CSI-2 electrical interface?
3. Does the connector plus main-board routing qualify as short/standard channel for `3.5 Gbps/lane`, or should the design target be limited to `2.5 Gbps/lane`?
4. Which A5EC pins are assigned to MIPI RZQ/refclk and are they free from LPDDR5 EMIF conflicts?

## P1: LPDDR5 EMIF Closure

1. Confirmed for Rev1: plan 2 groups of x32 LPDDR5 components; each group has one LPDDR5 hard memory controller.
2. Which exact LPDDR5 component and vendor datasheet will be used?
3. Does Quartus EMIF IP accept two x32 LPDDR5 controller groups on the exact A5EC device/package/speed grade at `3,733 Mbps/pin`?
4. For both controller groups, are address/command lanes, data byte lanes, RZQ, refclk, reset, and bank voltage assignments legal in pin planner?
5. What lower FSP values should be used for bring-up before attempting the target rate?

## P1: LM5060 Migration Closure

1. What are the old LM5060 circuit parameters and measured/proven operating envelope?
2. What is the new downstream bulk capacitance and startup load for Agilex 5 + LPDDR5 rails?
3. Do current limit, timer, hot-swap MOSFET SOA, TVS/fuse/EMI parts, and PG/FLT timing still have margin?

## P1: Tooling Issue

1. The initial board review hit `DiffPairCheck` missing `pair_name`. Should this be fixed in `sch-review` before relying on board-level findings?
2. Which subset of the current 40 P0 findings remains after that tool issue is fixed?

## P1: Requirements Inputs

1. Is there a `requirements.yaml` for this DF108 revision?
2. Is there a `system.yaml` or board-to-board interface contract?
3. Are EMC/high-speed constraints available for FAKRA, POC, DPS, optical, GTS, and DDR?

## Suggested Next Prompt For Another LLM

Given the context and facts above, first read `judgment_interpretation.md`. Treat the current input as a correct old schematic with a new Agilex package/scheme placeholder. Do not convert raw `errors=40` into confirmed design errors. Separate hard facts, user-stated task intent, placeholder TODOs, tool issues, missing evidence, and formal release blockers.
