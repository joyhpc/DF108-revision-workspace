# Schematic Rev1 Execution Plan

This file is a lightweight execution constraint page for the DF108 Rev1 schematic drafting task.

It is not schematic sign-off, board-release approval, or a formal design-freeze record. Load it only when the task is to continue Rev1 schematic planning, drawing order, work estimation, or first-pass schematic checking.

## Load-On-Demand Rule

Use this file when the user says things like:

- continue Rev1 schematic work;
- estimate or adjust schematic drawing time;
- decide the next schematic page to draw;
- check whether a schematic page is complete enough for first-pass review;
- keep future LLM output aligned with the current fast-first-version strategy.

Do not use this file as the main input for final sign-off, release approval, procurement freeze, SI/PI closure, or formal hardware closure. Those tasks need a separate evidence set.

## Current Design State Header

Every schematic-assist response should start with this state block:

```text
已确认:
暂定假设:
待补证:
当前要画的页:
```

Use short, concrete entries. Do not turn this block into a full review report.

## Rev1 Goal

The current goal is to finish a clear first schematic revision quickly.

In scope:

- replace the old KU040-centric controller path with the Agilex 5 Rev1 direction;
- keep the DF108 external/peripheral domain traceable;
- allocate major FPGA resources at a schematic-planning level;
- make open questions visible instead of blocking all drawing;
- leave enough evidence for the next review pass.

Out of scope for this pass:

- final pin/bank sign-off;
- final LPDDR5 EMIF closure;
- final MIPI channel/SI closure;
- final power sequencing closure;
- formal board-release approval.

## Four-Day Drawing Plan

Assume `0.5 day = 4 hours` and `1 day = 8 hours`.

| Day | Main target |
|---|---|
| Day 1 | System block diagram, power tree diagram, FPGA top-level symbol paging, GPIO bank allocation. |
| Day 2 | Two LPDDR5 x32 groups: part selection, package/symbol/footprint preparation, LPDDR5 module schematic, first-pass EMIF pin assignment. |
| Day 3 | Power input, power rails and sequencing, clock/reset/config, MIPI direct-connect update, preserved peripheral interfaces. |
| Day 4 | Full schematic check, netlist/BOM/package consistency check, GPIO/LPDDR5/MIPI/resource-matrix update, open-question update. |

Planning number:

- target drawing time: `4 working days`;
- management-facing range: `4-5 working days`;
- the fifth day is buffer for hard resource conflicts, not part of the nominal drawing task.

KU040 deletion is treated as quick cleanup inside the interface-preservation work. Do not estimate it as a standalone major workstream unless the schematic shows hidden dependency fan-out.

## Current Effective Technical Direction

Use these as Rev1 working assumptions:

- KU040 is removed in the target Rev1 schematic.
- The 168 decoder ordinary GPIO signals require adjustable `1.2 V` to `1.8 V` I/O banks.
- The 168 GPIO signals are grouped as four logical groups of 42 signals, targeting HSIO / `VCCIO_PIO` adjustable sub-banks.
- LPDDR5 uses two `x32` groups, with one LPDDR5 hard memory controller per group.
- MIPI removes the HS/LP switch and buffer, then routes decoder-board MIPI through the connector directly to Agilex 5 MIPI-capable HSIO.
- The LM5060 input-power circuit can be migrated structurally, but current limit, inrush, MOSFET SOA, `PG` / `FLT`, and downstream sequencing must be recalculated.
- `A5EC` / `A5ED` naming is not by itself a schematic error in this first-pass discussion, but it is a real resource-capacity risk because local pinout evidence shows different HSIO availability.

## Required Output Shape

For schematic-assist responses, use two layers:

### 技术层

Give drawing-useful details:

- page/module to draw;
- signal groups and intended ownership;
- rail names and sequencing assumptions;
- required labels, placeholders, and cross-probes;
- items that must remain pending until Quartus, Pin Planner, official Intel/Altera documentation, vendor datasheets, or reference designs confirm them.

### 决策层

Translate engineering state into schedule and risk:

- whether the drawing can continue;
- whether a topic blocks first-pass schematic work;
- expected rework if the assumption is wrong;
- what should be checked next.

Avoid sign-off language. Use "first-pass direction", "pending confirmation", "draw now / verify later", or "blocks drawing" instead of "closed" or "approved".

## Unknowns That Must Stay Marked

Do not infer these from memory or from generic FPGA knowledge:

- exact Agilex 5 bank and ball assignment;
- LPDDR5 EMIF legal pin plan and byte-lane placement;
- MIPI D-PHY lane placement, RZQ/refclk constraints, and maximum usable lane rate;
- power rail sequencing limits and allowable ramp dependencies;
- final `A5EC` versus `A5ED` ordering name and package-specific resource table.

Mark them as pending Quartus / Pin Planner / official datasheet / reference design confirmation.

## Load With These Files When Needed

For normal Rev1 schematic continuation, load:

1. `02_key_facts.md`
2. `03_open_questions.md`
3. `04_current_design_direction.md`
4. `05_schematic_rev1_execution_plan.md`

For resource allocation work, also load:

1. `../02_design_evidence/a5ec052a_b32a_resource_allocation_matrix_20260507.csv`
2. `../02_design_evidence/ku040_removal_gpio_bank_allocation_20260508.md`
3. `../02_design_evidence/current_design_direction_20260507.md`

For historical review interpretation, use `LLM_NAVIGATION.md` and the current report index instead of this file.

## First-Pass Completion Criteria

The Rev1 schematic is first-pass complete when:

- all planned pages exist and have clear ownership;
- LPDDR5, MIPI, GPIO, power, clock, reset, config, and external interfaces are represented;
- GPIO count and grouping are traceable;
- LPDDR5 has two x32 groups and one controller per group shown clearly;
- MIPI direct-connect topology is shown without the removed switch/buffer path;
- power rails and sequencing dependencies are labeled, even if some values remain pending;
- the resource matrix and open-question list are updated;
- no output claims final sign-off or formal closure.
