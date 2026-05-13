# DF108 LPDDR5 / LPDDR5X Selection Map

## Metadata

| Field | Value |
|---|---|
| Project | DF108 / A38 Agilex 5 migration |
| Revision | `rev-20260506-df108-ku040-to-a5ed052ab32ae2v` |
| Component / function | External memory, 2 groups of x32 LPDDR5/LPDDR5X components |
| Map date | 2026-05-08 |
| Related decision record | `20260508-lpddr5-selection.md` |
| Map owner | Hardware owner, with procurement and logic inputs |
| Review date | 2026-05-13 |

## Map Purpose

This map is the navigation layer for continuing the LPDDR5/LPDDR5X selection. It does not replace the decision record. It preserves the source routes, candidate funnel, rejection reasons, evidence gaps, evidence-acquisition channels, and tool-validation path needed to move the current `selected-not-frozen` decision toward freeze or back to architecture review.

The map intentionally avoids listing every public SKU. It keeps exact part numbers only where they are decision-relevant, supplier-follow-up targets, or Quartus/hardware validation inputs.

## Source Map

| Source ID | Source type | Title / description | Date | Path / URL / owner | Trust level | Candidate route | Supports which conclusion | Status |
|---|---|---|---|---|---|---|---|---|
| S1 | project evidence report | A38 / DF108 LPDDR5 procurement engineering evidence report | 2026-05-08 | `/home/ubuntu/my-daily/Daily/raw/2026-05-08/5月8日_extracted/lpddr5_report_engineering_evidence.md` | project | All routes | Consolidates Gmail, datasheet extracts, PCN extracts, and engineering gates. | active |
| S2 | project decision report | A38 / DF108 LPDDR5 procurement internal decision report | 2026-05-08 | `/home/ubuntu/my-daily/Daily/raw/2026-05-08/5月8日_extracted/lpddr5_report_decision.md` | project | All routes | Establishes Micron primary direction and non-freeze status. | active |
| S3 | procurement report | LPDDR5 procurement communication report | 2026-05-08 | `/home/ubuntu/my-daily/Daily/raw/2026-05-08/5月8日_extracted/lpddr5_report_procurement.md` | project | Micron primary, Samsung watchlist, Henry/Hynix watchlist | Provides supplier question list and email drafts. | active |
| S4 | project note | LPDDR5 pin assignment / pin placement pointers | 2026-05-08 | `/home/ubuntu/my-daily/Daily/raw/2026-05-08/5月8日_extracted/LPDDR5 PIN ASSIGN.md` | project | Tool validation | Points to Altera/Intel EMIF User Guide LPDDR5 support and pin-placement sections. | active |
| S5 | handoff facts | DF108 migration key facts | 2026-05-08 | `../06_llm_handoff/02_key_facts.md` | project | Architecture/resource closure | Captures A5ED target, two x32 LPDDR5 plan, 3733 Mbps/pin target, and resource caution. | active |
| S6 | handoff open questions | DF108 open questions | 2026-05-08 | `../06_llm_handoff/03_open_questions.md` | project | Architecture/resource closure | Captures P0 GPIO/HSIO and P1 LPDDR5 EMIF closure questions. | active |
| S7 | design direction | Current design direction update | 2026-05-07 | `../02_design_evidence/current_design_direction_20260507.md` | project | Architecture/resource closure | Explains MIPI, LPDDR5, and 168 adjustable GPIO coexistence risk. | active |
| S8 | supplier email pointer | Kun Cao / WT Microelectronics recommends Micron 4GB x32 candidate | 2026-05-08 | Gmail ID `19e065cdbd67077e`, summarized in S1/S2 | supplier | Micron primary | Gives exact Micron candidate and project-info request. | active |
| S9 | supplier email pointer | Vince Huo / WPI provides Micron PCN and 9600 MT/s direction | 2026-05-08 | Gmail ID `19e065df94f3cfec`, summarized in S1/S2 | supplier | Micron primary, old route rejection | Supports 9600 direction and older-speed EOL risk. | active |
| S10 | supplier email pointer | Link Liu / Golden Supreme Samsung LP5X feedback | 2026-05-08 | Gmail ID `19e065c771a63d06`, summarized in S1/S2 | supplier | Samsung 245FBGA rejected route | Supports rejection of the 245FBGA consumer route for this project. | active |
| S11 | supplier email pointer | Fifi Lin / WT Microelectronics says Nanya has no LPDDR5 | 2026-05-08 | Gmail ID `19e065d03c1d5052`, summarized in S1/S2 | supplier | Nanya closed route | Closes Nanya route. | active |
| S12 | supplier email pointer | Procurement request sent to Henry / HSRP, no reply in searched range | 2026-05-08 | Gmail ID `19e065c87163f67f`, summarized in S1/S2 | supplier | Henry/Hynix watchlist | Shows the channel was asked but has not answered. | active |
| S13 | datasheet extract | Micron Y62P LPDDR5X SDRAM datasheet extract, Rev. G 03/2026 | 2026-03 | Attachment `315b-441b-561b-y62p-ddp-qdp-8dp-non-auto-lpddr5x.pdf`, summarized in S1 | primary via extract | Micron primary | Supports x32, 4GB / 32Gb, LPDDR5X/LPDDR5 data interface, 9600 Mb/s per pin, 315-ball TFBGA DS. | active |
| S14 | PCN extract | Micron PCN 36290, EOL for Y52P specific 315b packages | Published 2026-02-04 | Attachment `PCN 36290.pdf`, summarized in S1/S2 | primary via extract | Old 2GB / old-generation route | Rejects old Y52P 315b direction for long-life freeze. | active |
| S15 | PCN pointer | Micron PCN 36383 referenced in supplier email | Published 2026-04-22 | Email body summarized in S1/S2 | supplier | Old 2GB / old-generation route | Supports Y52Q 2GB x32 EOL risk; full PCN is still needed if used as formal freeze evidence. | active |
| S16 | team update | LPDDR5 group feedback and Samsung 315FBGA public-candidate note | 2026-05-08 | `/home/ubuntu/my-daily/Daily/raw/2026-05-08/5月8日_extracted/lpddr5 情况群内反馈.md` | project / secondary | Samsung 315FBGA watchlist | Identifies Samsung 32Gb x32 315FBGA public-candidate route for formal follow-up. | active |
| S17 | team update | Concise LPDDR5 action-item update | 2026-05-08 | `/home/ubuntu/my-daily/Daily/raw/2026-05-08/5月8日_extracted/lpddr5 情况群内反馈 2.md` | project | Action owners | Captures procurement, project, logic, and hardware action split. | active |
| D1 | decision record | DF108 LPDDR5 / LPDDR5X component selection decision | 2026-05-08 | `20260508-lpddr5-selection.md` | project | All routes | Current selected-not-frozen decision and freeze blockers. | active |

## Candidate Funnel

| Funnel class | Route / family / exact candidate | Representative exact PN if needed | Why this level is enough | Evidence pointer | Next action |
|---|---|---|---|---|---|
| Primary | Micron Y62P 32Gb x32 LPDDR5X 315-ball TFBGA DS route | `MT62F1G32D2DS-020 WT:D` | Exact PN is needed for procurement, EMIF input, symbol/footprint, and supplier questions. | S1/S2/S8/S9/S13/D1 | Continue as validation primary; do not freeze. |
| Backup | None confirmed | N-A | No route has enough formal lifecycle, package, commercial, and validation evidence to be called backup. | D1 | Promote only after evidence matrix can cite formal sources. |
| Watchlist | Samsung 32Gb x32 315FBGA LPDDR5X route | `K3KL8L80QM-MFCT`, `K3KL8L80CM-MGCT` as procurement follow-up targets | Exact PN examples are useful to ask formal Samsung channels; do not list every Samsung variant. | S16/S17/D1 | Ask formal channel for lifecycle, commercial terms, package, and availability. |
| Watchlist | Henry / HSRP / Hynix LPDDR5/LPDDR5X route | TBD-evidence | No reply yet; route is still worth one follow-up because Hynix is a first-tier vendor. | S12/S17/D1 | Follow up once; classify answer as backup, rejected, or closed. |
| Watchlist | New 2GB x32 long-life route from any first-tier vendor | TBD-evidence | Original requirement is 2GB per component, but current old-generation evidence is poor. Keep only as a route-level question. | S1/S2/S3/D1 | Ask suppliers whether any non-EOL, long-life 2GB x32 part exists. |
| Rejected | Old-generation Micron/Y52 2GB x32 direction | Exact PN not needed for current path | EOL/PCN evidence conflicts with 5-8 year lifecycle target. | S14/S15/D1 | Reopen only with a new exact non-EOL replacement and formal lifecycle statement. |
| Rejected | Samsung 245FBGA consumer route | `K3KL8L80DM-TGCT` | Exact PN matters because supplier evidence specifically points to this rejected route. | S10/D1 | Reopen only if Samsung supplies a long-life compatible package/route. |
| Closed | Nanya route | N-A | Supplier says no LPDDR5. | S11/D1 | Reopen only if Nanya or distributor formally updates product availability. |

## Requirement Coverage Map

Allowed status values: `confirmed`, `TBD-evidence`, `conflict`, `N-A`.

| Requirement / gate | Primary route status | Backup / watchlist status | Evidence pointer | Status | Freeze impact |
|---|---|---|---|---|---|
| x32 component width | Micron primary is x32. | Samsung 245FBGA is x32; Samsung 315FBGA public route claims x32 but needs formal evidence. | S1/S8/S10/S13/S16 | confirmed | Width itself does not block primary validation. |
| Original 2GB / 16Gb per component capacity | Micron primary is 4GB / 32Gb. | Viable long-life 2GB route is not proven. | S1/S2/S3/S13/D1 | conflict | Requires project owner capacity-change approval before freeze. |
| 2 groups x32, 8GB total if Micron is used | Primary implies 2 x 4GB = 8GB total. | Same likely for Samsung 32Gb watchlist. | S16/S17/D1 | TBD-evidence | Project owner must approve cost/software/power impact. |
| LPDDR5 / LPDDR5X interface suitability | Micron datasheet extract says LPDDR5X/LPDDR5 data interface. | Samsung watchlist is not formally confirmed for this project. | S1/S13/S16 | confirmed | Allows engineering evaluation, not freeze. |
| 3733 Mbps/pin derated operation | Micron is 9600 Mb/s per pin; derating guidance not confirmed. | Samsung watchlist also needs derating confirmation. | S1/S2/S3/S13 | TBD-evidence | Blocks freeze until supplier guidance and Quartus validation exist. |
| 5-8 year lifecycle / no known EOL | Exact Micron Y62P lifecycle not confirmed. | Old 2GB route conflicts; Samsung watchlist unknown. | S1/S2/S9/S14/S15/S16 | TBD-evidence | Blocks freeze. |
| Commercial terms | No Micron price, lead time, MOQ, or MPQ recorded. | Watchlist routes also lack formal terms. | S3/D1 | TBD-evidence | Blocks BOM freeze. |
| Temperature / supply grade | `WT:D` meaning not formally confirmed. | Samsung watchlist temperature data from project note is not formal channel evidence. | S1/S3/S13/S16 | TBD-evidence | Blocks freeze. |
| Package / footprint / pinout | Micron package identity is known as 315-ball TFBGA DS; DF108 symbol/footprint/pinout not checked. | Samsung 245FBGA conflicts; Samsung 315FBGA watchlist needs formal package data. | S1/S4/S10/S13/S16/D1 | TBD-evidence | Blocks schematic/package/pin freeze. |
| Quartus EMIF / Pin Planner / Fitter | No artifact yet. | No artifact yet. | S4/S5/S6/S7/D1 | TBD-evidence | Blocks freeze and may force architecture change. |
| `MIPI + 2x LPDDR5 x32 + 168 adjustable GPIO` resource coexistence | Not proven and currently high risk for A5ED B32A. | Same architecture risk applies to all memory routes. | S5/S6/S7/D1 | TBD-evidence | P0 blocker; can invalidate memory route regardless of supplier. |

## Rejection Ledger

| Route / candidate | Rejection reason | Evidence pointer | Reopen condition | Owner |
|---|---|---|---|---|
| Old-generation Micron/Y52 2GB x32 route | PCN/EOL evidence conflicts with 5-8 year lifecycle target. | S14/S15/D1 | Supplier provides a new exact 2GB x32 non-EOL part with formal lifecycle and commercial evidence. | Procurement |
| Samsung `K3KL8L80DM-TGCT` 245FBGA route | Supplier describes consumer lifecycle around 2-3 years; package differs from 315-ball direction; not a clean substitute. | S10/D1 | Formal Samsung channel provides a long-life part/package path and supplier evidence that satisfies freeze gates. | Procurement |
| Nanya route | Supplier feedback says Nanya has no LPDDR5. | S11/D1 | Nanya or authorized distributor formally confirms a suitable LPDDR5/LPDDR5X product. | Procurement |
| Treating Samsung 315FBGA public SKUs as backup | Evidence is project/secondary, not formal supplier confirmation. | S16/S17/D1 | Formal Samsung channel confirms exact PN, lifecycle, commercial terms, and package data. | Procurement |
| Freezing LPDDR5 pin list now | Quartus EMIF, Pin Planner, Fitter, package, and resource-coexistence evidence are missing. | S1/S4/S5/S6/S7/D1 | Required tool and hardware artifacts pass or produce an accepted architecture change. | Logic + hardware |

## Open Evidence Ledger

| Evidence gap | Affects gate | Current best route | Needed evidence format | Owner | Due / review date | Status |
|---|---|---|---|---|---|---|
| Exact Micron lifecycle / EOL posture for `MT62F1G32D2DS-020 WT:D` | Lifecycle freeze gate | Micron primary | Vendor lifecycle statement, PCN/EOL search result, or supplier email with exact PN and date | Procurement | 2026-05-13 | TBD-evidence |
| `WT:D` temperature and supply grade meaning | Temperature / grade gate | Micron primary | Datasheet table or vendor/supplier email with exact PN | Procurement | 2026-05-13 | TBD-evidence |
| Sample lead, MP lead, price ladder, MOQ, MPQ | Commercial gate | Micron primary | Quote or supplier email with exact PN and date | Procurement | 2026-05-13 | TBD-evidence |
| 9600 Mb/s part running at 3733 Mbps/pin | Derating and SI/tool gate | Micron primary | Micron/FAE guidance plus Quartus validation artifact | Procurement + logic | 2026-05-13 | TBD-evidence |
| Capacity increase from 4GB total to 8GB total | Requirement-change gate | Micron primary and Samsung 32Gb watchlist | Project owner signoff or requirement update | Project owner / 罗奇军 | 2026-05-13 | TBD-evidence |
| Quartus EMIF support for two x32 groups | Toolchain gate | All usable routes | EMIF config/export for exact target | Logic / 吴志安 | 2026-05-12 | TBD-evidence |
| Pin Planner/Fitter resource coexistence | Architecture/resource gate | All usable routes | Pin Planner, Fitter, QSF/pin report, and conflict statement | Logic / 吴志安 | 2026-05-12 | TBD-evidence |
| Micron 315-ball DS symbol/footprint feasibility | Package/library gate | Micron primary | Library review, package drawing reference, footprint check | Hardware | 2026-05-14 | TBD-evidence |
| Samsung 315FBGA formal route | Backup / second-source gate | Samsung watchlist | Formal supplier response, datasheet, lifecycle and commercial statement | Procurement | 2026-05-15 | TBD-evidence |
| Henry/Hynix response | Backup / second-source gate | Henry/Hynix watchlist | Supplier reply or explicit no-response record | Procurement | 2026-05-15 | asked |

## Evidence Acquisition Plan

Allowed status values: `to-ask`, `asked`, `answered`, `stale`, `blocked`, `N-A`.

| Evidence gap | Best channel | Who asks | Question to ask | Required answer format | Status |
|---|---|---|---|---|---|
| Exact Micron lifecycle / EOL posture | Original vendor or authorized distributor | Procurement | For exact PN `MT62F1G32D2DS-020 WT:D`, is there any known PCN/EOL risk, and can it support the project 5-8 year horizon? | Dated email or official vendor/distributor statement with exact PN; PCN/EOL document if applicable. | to-ask |
| `WT:D` grade meaning | Original vendor or authorized distributor FAE | Procurement | What temperature range and supply/quality grade does `WT:D` mean for this exact PN? | Datasheet table, ordering-code table, or dated supplier/FAE email. | to-ask |
| Commercial terms | Authorized distributor / procurement | Procurement | What are sample lead time, MP lead time, price ladder, MOQ, and MPQ for the exact PN? | Quote or dated supplier email with exact PN and validity window. | to-ask |
| 3733 Mbps/pin derating guidance | Original vendor FAE plus internal logic validation | Procurement + logic | Does the 9600 Mb/s per-pin LPDDR5X part support long-term operation at 3733 Mbps/pin, and are there ODT, training, SI, initialization, or mode-register caveats? | FAE email or app note plus Quartus EMIF/Pin Planner/Fitter artifacts. | to-ask |
| Capacity increase acceptance | Internal project owner | Hardware / project owner | Can DF108 accept 2 x 4GB x32 parts, making total memory 8GB instead of planned 4GB? | Project signoff or requirement update covering BOM cost, software, init, power, and thermal impact. | to-ask |
| Quartus exact-device placement | Internal logic/tool path | Logic / 吴志安 | Can exact B32A target place two x32 LPDDR5 groups at 3733 Mbps/pin together with MIPI and 168 adjustable GPIO? | EMIF export, Pin Planner output, Fitter report, QSF/pin report, conflict statement. | to-ask |
| Samsung 315FBGA long-life option | Samsung formal channel / authorized distributor | Procurement | Are `K3KL8L80QM-MFCT`, `K3KL8L80CM-MGCT`, or a related 32Gb x32 315FBGA LPDDR5X part available with suitable lifecycle and commercial terms? | Dated supplier response, datasheet, quote, lifecycle/PCN statement. | to-ask |
| Hynix / Henry route | Henry / HSRP or other Hynix distributor | Procurement | Is there a 2GB x32 long-life part, or a 4GB x32 315FBGA-class LPDDR5/LPDDR5X alternative? | Dated reply with exact PN, availability, lifecycle, package, and commercial terms, or explicit no-bid. | asked |

## Tool Validation Map

| Validation item | Inputs | Tool / method | Owner | Pass criteria | Output artifact | Status |
|---|---|---|---|---|---|---|
| EMIF configuration feasibility | Exact Agilex 5 target, two x32 LPDDR5/LPDDR5X groups, 3733 Mbps/pin, Micron primary first | Quartus EMIF IP | Logic / 吴志安 | Configuration is accepted for exact device/package/speed grade without unsupported parameter combinations. | EMIF config screenshot/export | TBD-evidence |
| Pin placement legality | EMIF output, LPDDR5 address/command/data byte lanes, RZQ, refclk, reset, target banks | Quartus Pin Planner | Logic / 吴志安 | Both x32 groups have legal pin placement and required resources. | Pin Planner output and pin report | TBD-evidence |
| Full resource coexistence | MIPI, 2 x x32 LPDDR5, 168 adjustable 1.2-1.8 V GPIO, clocks, resets, config, QSFP if relevant | Quartus Fitter / resource planning | Logic / 吴志安 | Fitter passes or provides an explicit conflict list that can drive architecture decision. | Fitter report, QSF, conflict statement | TBD-evidence |
| Package/library feasibility | Micron 315-ball TFBGA DS package, preliminary symbol, footprint, power pins, reset, RZQ/ZQ, refclk, ODT/VREF handling | Hardware library review | Hardware | Symbol and footprint can be built without missing package evidence; no pinout mismatch against EMIF plan. | Symbol/footprint feasibility note | TBD-evidence |
| SI/PI/layout feasibility | 315-ball package, target speed, routing layers, impedance, length matching, power rails, decoupling, board space | Hardware SI/PI precheck | Hardware | Escape and routing strategy are plausible before schematic/pin freeze; blockers are named. | SI/PI/layout precheck | TBD-evidence |
| Bring-up strategy | Lower FSP options, memory initialization/training, board test plan | Logic + hardware review | Logic + hardware | Bring-up can start below target rate and progress to 3733 Mbps/pin with measurable checkpoints. | Bring-up plan | TBD-evidence |

## Update Rules

- Promote Samsung or Hynix from `Watchlist` to `Backup` only after formal supplier evidence covers exact PN, lifecycle, commercial terms, package, and basic engineering inputs.
- Promote Micron from `selected-not-frozen` toward freeze only after capacity approval, supplier evidence, Quartus artifacts, and hardware package/SI checks are available.
- Reopen 2GB only if a supplier produces an exact non-EOL x32 part with 5-8 year lifecycle evidence.
- Mark any price, lead-time, lifecycle, PCN, or tool-version evidence stale when its validity window, PCN status, or tool release changes.
- Keep raw emails, datasheets, PCNs, and Quartus outputs in project evidence storage; this map only points to them and summarizes decision impact.
