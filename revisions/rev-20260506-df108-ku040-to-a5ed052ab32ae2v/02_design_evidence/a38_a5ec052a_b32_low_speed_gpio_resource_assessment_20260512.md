# A38 / A5EC052A B32 Low-Speed GPIO Resource Assessment Summary

This Markdown page mirrors the review-critical conclusions from [a38_a5ec052a_b32_low_speed_gpio_resource_assessment_20260512.xlsx](a38_a5ec052a_b32_low_speed_gpio_resource_assessment_20260512.xlsx) so GitHub reviewers can read the current GPIO state without opening Excel.

Status: `TBD-evidence`, not sign-off.

## Current Conclusion

The current count-based GPIO view is usable for Rev1 planning, but it is not enough for freeze. Ordinary low-speed GPIO demand is `205`; counted A5E remaining resources are `256`; the theoretical pin-level margin is `51`. This means the project can continue resource planning, but it must not claim voltage-domain closure until VDDIO semantics, bank granularity, and tool reports are checked.

## Technical Layer

| Item | Current evidence / assumption | Status | Review note |
|---|---|---|---|
| High-speed allocation boundary | LPDDR5 and MIPI have already been assigned in HSIO under the current design premise. | assumed current baseline | Do not double-count these HSIO resources for ordinary GPIO without Quartus evidence. |
| QSFP boundary | QSFP high-speed side has already been assigned in GTS. | assumed current baseline | GTS ordinary low-speed GPIO resource is counted as `0`. QSFP low-speed management signals still need 3.3 V GPIO. |
| Low-speed GPIO demand | Total ordinary low-speed GPIO demand is `205`. | current count | `168` decoder board GPIO plus `37` 3.3 V low-speed control GPIO. |
| Counted resource total | A5E counted low-speed GPIO resources total `256`. | current count | Sum is HVIO `120` + HSIO 2A `26` + HSIO 2B/3A `24` + HSIO 3B right `48` + HSIO 3B left `38` + GTS `0`. |
| Theoretical margin | `256 - 205 = 51`. | count-only margin | This does not account for bank VCCIO grouping, fixed-voltage resources, placement legality, or Fitter conflicts. |
| 3.3 V control GPIO | 3.3 V GPIO should preferentially use HVIO. | recommended allocation | Includes decoder power EN, PMU, QSFP management, I2C, DEV ID, and external expansion IO. |
| Decoder board GPIO | `168` GPIO require VDDIO configurable from `1.2 V` to `1.8 V`. | key risk | Fixed `1.2 V` HSIO and LPDDR5 same-voltage resources cannot automatically satisfy full-range adjustable VDDIO. |
| Strict adjustable interpretation | Under strict per-signal `1.2 V` to `1.8 V` adjustability, closure still needs 3B right, HVIO bank granularity, and Pin Planner/Fitter confirmation. | `TBD-evidence` / risk | If 3B right cannot follow decoder VADJ, the resource gap grows; if HVIO is consumed by 3.3 V GPIO, VADJ capacity shrinks. |

## Resource Count Snapshot

| Resource | Count | Voltage / usage note | Current use guidance |
|---|---:|---|---|
| HVIO Bank x6 | 120 | Adjustable `1.2 V` to `3.3 V` by bank | First choice for `37` 3.3 V GPIO; possible VADJ support depends on bank grouping. |
| HSIO Bank 2A | 26 | Fixed `1.2 V` | Usable only if decoder GPIO can be fixed to `1.2 V` in this revision. |
| HSIO Bank 2B / 3A | 24 | Same-voltage context with LPDDR5 | Needs Quartus EMIF, Pin Planner and Fitter evidence before counting as GPIO. |
| HSIO Bank 3B right half | 48 | VDDIO / mux restrictions to confirm | Critical resource for a strict decoder VADJ path. |
| HSIO Bank 3B left half | 38 | Fixed `1.2 V` | Same limitation as fixed 1.2 V resources. |
| GTS | 0 | QSFP high-speed already assigned | Do not allocate ordinary low-speed GPIO to GTS. |

## Decision Layer

| Decision question | Current answer | Owner | Next action |
|---|---|---|---|
| Can PM say GPIO quantity is enough? | Only at count-planning level: `256` counted resources versus `205` demand, margin `51`. | Hardware | Keep as planning evidence, not closure. |
| Can PM say GPIO is sign-off ready? | No. Voltage-domain compatibility and tool placement are not closed. | Project owner + hardware + logic | Keep GPIO as `TBD-evidence` until Pin Planner/Fitter and VDDIO decisions exist. |
| What is the main schedule risk? | The `168` decoder board GPIO may require full `1.2 V` to `1.8 V` adjustability. If resources are drawn with fixed 1.2 V assumptions and the requirement later stays strict, schematic and layout work can be reworked. | Project owner + requirements / architecture | Decide whether this revision truly needs every decoder GPIO to support full-range VADJ. |
| What is the fastest blocker to clear? | Confirm HSIO 3B right VDDIO behavior and HVIO bank granularity, then run a Pin Planner/Fitter coarse assignment. | FPGA / logic | Produce bank report, Pin Planner output, Fitter report or explicit conflict list. |
| What mitigation paths exist if strict VADJ does not close? | Move some 3.3 V control GPIO to an I/O expander, CPLD, MCU or bridge; add level shifting or split decoder GPIO groups; reduce GPIO demand; or change FPGA/package. | Project owner + hardware + logic | Choose mitigation only after tool evidence shows the actual gap. |

## Required Closure Evidence

| Evidence | Owner | Status |
|---|---|---|
| Definition of decoder board VDDIO requirement: full-range per signal versus this-revision fixed voltage | Requirements / architecture | open |
| HSIO 3B right VDDIO and mux limitation check | FPGA / Pin Planner | open |
| HVIO bank-by-bank VCCIO and available-pin report | FPGA / layout | open |
| Quartus Pin Planner coarse assignment for `DEC_GPIO[167:0]` and `GPIO_3V3_CTRL[36:0]` | Logic | open |
| Fitter pass or explicit conflict report with LPDDR5, MIPI, QSFP/GTS and ordinary GPIO constraints together | Logic | open |
| Schematic page split for decoder GPIO, 3.3 V controls, and power sequencing | Hardware | open |
