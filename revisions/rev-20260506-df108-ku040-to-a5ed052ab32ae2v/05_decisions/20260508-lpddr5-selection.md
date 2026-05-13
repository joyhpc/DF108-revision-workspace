# DF108 LPDDR5 / LPDDR5X Component Selection Decision

## Metadata

| Field | Value |
|---|---|
| Project | DF108 / A38 Agilex 5 migration |
| Revision | `rev-20260506-df108-ku040-to-a5ed052ab32ae2v` |
| Component / function | External memory, 2 groups of x32 LPDDR5/LPDDR5X components |
| Decision date | 2026-05-08 |
| Decision owner | Project owner for capacity change; hardware owner for schematic/package; logic owner for Quartus closure; procurement for supplier evidence |
| Review date | 2026-05-13 |
| Record status | selected-not-frozen |

## Decision Objective

Decide whether DF108 should proceed with a primary LPDDR5/LPDDR5X component for procurement and engineering validation before schematic/BOM/pin-list freeze.

This record answers the current practical question:

- Can the project use Micron `MT62F1G32D2DS-020 WT:D` as the primary candidate now?
- Which candidates are rejected or only watchlist?
- What exact evidence must exist before LPDDR5/LPDDR5X is allowed to freeze into schematic, BOM, pin assignment, and PCB constraints?

## Entry Phase

Existing shortlist plus pre-freeze review.

Reason: supplier feedback has already produced one concrete Micron candidate, rejected several routes, and exposed freeze blockers. The correct output is not a fresh search brief; it is a selected-not-frozen decision with explicit evidence gaps and engineering gates.

## Source Inventory

| Source ID | Type | Title / description | Date | Owner / path / URL | Trust level | Notes |
|---|---|---|---|---|---|---|
| S1 | Project evidence report | A38 / DF108 LPDDR5 procurement engineering evidence report | 2026-05-08 | `/home/ubuntu/my-daily/Daily/raw/2026-05-08/5月8日_extracted/lpddr5_report_engineering_evidence.md` | project | Consolidates Gmail, datasheet extracts, PCN extracts, and engineering recommendations. |
| S2 | Project decision report | A38 / DF108 LPDDR5 procurement internal decision report | 2026-05-08 | `/home/ubuntu/my-daily/Daily/raw/2026-05-08/5月8日_extracted/lpddr5_report_decision.md` | project | Summarizes the procurement decision direction and action list. |
| S3 | Procurement report | LPDDR5 procurement communication report | 2026-05-08 | `/home/ubuntu/my-daily/Daily/raw/2026-05-08/5月8日_extracted/lpddr5_report_procurement.md` | project | Contains supplier questions and draft emails. |
| S4 | EMIF pin-placement pointer | LPDDR5 pin assignment and Altera/Intel EMIF guide locations | 2026-05-08 | `/home/ubuntu/my-daily/Daily/raw/2026-05-08/5月8日_extracted/LPDDR5 PIN ASSIGN.md` | project | Points to EMIF User Guide 817467_D842785 and official online LPDDR5 support pages. |
| S5 | Project key facts | DF108 migration key facts | 2026-05-08 | `../06_llm_handoff/02_key_facts.md` | project | Captures A5ED target, LPDDR5 topology, 3733 Mbps/pin target, and resource caution. |
| S6 | Project open questions | DF108 open questions | 2026-05-08 | `../06_llm_handoff/03_open_questions.md` | project | Captures LPDDR5 EMIF closure and P0 GPIO/HSIO resource questions. |
| S7 | Design direction | Current design direction update | 2026-05-07 | `../02_design_evidence/current_design_direction_20260507.md` | project | Captures two x32 LPDDR5 controller plan and MIPI/GPIO/LPDDR5 coexistence risk. |
| S8 | Supplier email pointer | Kun Cao / WT Microelectronics recommends Micron 4GB x32 candidate | 2026-05-08 | Gmail ID `19e065cdbd67077e`, summarized in S1/S2 | supplier | Raw email should be retained for freeze evidence. |
| S9 | Supplier email pointer | Vince Huo / WPI provides Micron PCN and 9600 MT/s direction | 2026-05-08 | Gmail ID `19e065df94f3cfec`, summarized in S1/S2 | supplier | Raw email and attachments should be retained for freeze evidence. |
| S10 | Supplier email pointer | Link Liu / Golden Supreme Samsung LP5X feedback | 2026-05-08 | Gmail ID `19e065c771a63d06`, summarized in S1/S2 | supplier | Rejects the 245FBGA consumer route for this project. |
| S11 | Supplier email pointer | Fifi Lin / WT Microelectronics says Nanya has no LPDDR5 | 2026-05-08 | Gmail ID `19e065d03c1d5052`, summarized in S1/S2 | supplier | Used to close the Nanya route. |
| S12 | Supplier email pointer | Procurement request sent to Henry / HSRP, no reply in searched range | 2026-05-08 | Gmail ID `19e065c87163f67f`, summarized in S1/S2 | supplier | This is not a usable candidate source yet. |
| S13 | Datasheet extract | Micron Y62P LPDDR5X SDRAM datasheet extract, Rev. G 03/2026 | 2026-03 | Attachment `315b-441b-561b-y62p-ddp-qdp-8dp-non-auto-lpddr5x.pdf`, summarized in S1 | primary via extract | Full attachment must be linked or archived before formal freeze. |
| S14 | PCN extract | Micron PCN 36290, EOL for Y52P specific 315b packages | Published 2026-02-04 | Attachment `PCN 36290.pdf`, summarized in S1/S2 | primary via extract | Confirms old Y52P route risk, not Y62P long-life approval. |
| S15 | PCN pointer | Micron PCN 36383 referenced in supplier email | Published 2026-04-22 | Email body summarized in S1/S2 | supplier | Full PCN PDF is required before freeze if used as formal evidence. |
| S16 | Team update | LPDDR5 group feedback and Samsung 315FBGA public-candidate note | 2026-05-08 | `/home/ubuntu/my-daily/Daily/raw/2026-05-08/5月8日_extracted/lpddr5 情况群内反馈.md` | project / secondary | Useful watchlist input; not a freeze-grade supplier confirmation. |
| S17 | Team update | Concise LPDDR5 action-item update | 2026-05-08 | `/home/ubuntu/my-daily/Daily/raw/2026-05-08/5月8日_extracted/lpddr5 情况群内反馈 2.md` | project | Captures owners and no-pin-freeze instruction. |

## Requirement Baseline

Hard constraints:

- Memory function must support the DF108 Agilex 5 memory architecture: 2 groups of x32 LPDDR5/LPDDR5X components, one LPDDR5 hard memory controller per group. Evidence: S5, S7.
- FPGA-side design target is 3733 Mbps/pin for the current Agilex 5 B32A direction. Higher EMIF menu values are not accepted without exact-device Quartus closure. Evidence: S5, S7.
- Each component must be x32. Evidence: original procurement requirement summarized in S1/S2/S3.
- The project target is 5-8 years without known EOL risk. Lifecycle, PCN, lead time, MOQ/MPQ, and price cannot be inferred from memory; they require supplier, vendor, distributor, or PCN evidence. Evidence: S1/S2/S3.
- LPDDR5/LPDDR5X pin list, bank assignment, and package footprint must not freeze until Quartus EMIF, Pin Planner, Fitter, package, power, and SI feasibility evidence exists. Evidence: S1/S4/S5/S6/S7.
- Final B32A resource closure must include `MIPI + 2x LPDDR5 x32 + 168 adjustable 1.2-1.8 V GPIO`. Evidence: S5/S6/S7.

Changeable constraints:

- Original capacity was 2GB / 16Gb per x32 component. It may change to 4GB / 32Gb per x32 component only if the project owner accepts the board-level capacity increase from 4GB total to 8GB total and the BOM, software, initialization, power, and thermal impacts. Evidence: S1/S2/S16/S17.
- Original wording prefers LPDDR5. LPDDR5X can be evaluated if the data interface is compatible and 3733 Mbps/pin derated operation is confirmed by supplier guidance and Quartus validation. Evidence: S1/S2/S13.
- Samsung 315FBGA parts can remain in the watchlist, but they are not a backup until formal channel evidence confirms lifecycle, commercial terms, availability, and package/pin compatibility. Evidence: S16.

Acceptance criteria before freeze:

- Primary and backup/watchlist classes are explicit.
- Supplier formally confirms lifecycle, PCN/EOL posture, temperature/supply grade, sample lead time, production lead time, price ladder, MOQ, and MPQ for the exact part number.
- Project owner signs off the capacity change if the primary remains 4GB per component.
- Logic owner provides Quartus EMIF configuration/export, Pin Planner output, Fitter report, QSF/pin report, and resource-conflict statement for the exact device/package/speed-grade target.
- Hardware owner confirms symbol, 315-ball TFBGA DS footprint, rail/RZQ/reset/refclk/ODT/VREF handling, PCB escape, SI/PI feasibility, and board-space impact.
- Procurement either identifies a valid 2GB x32 long-life alternative or records why the 2GB requirement is superseded.

## Candidate Classification

| Class | Candidate | Evidence pointer | Rationale |
|---|---|---|---|
| Primary | Micron `MT62F1G32D2DS-020 WT:D` | S1/S2/S8/S9/S13 | Only concrete first-tier candidate with a specific part number, x32 width, 4GB / 32Gb capacity, LPDDR5X/LPDDR5 data-interface evidence, 9600 Mb/s per-pin rating, and 315-ball TFBGA DS package evidence. It conflicts with the original 2GB capacity requirement and still lacks lifecycle, WT:D grade, commercial, derating, and Quartus evidence, so it is selected-not-frozen only. |
| Backup | None confirmed | S1/S2/S16 | No candidate currently satisfies evidence requirements for backup status. A backup must have at least part-number, x32 width, package, lifecycle path, commercial path, and formal source evidence. |
| Rejected | Original 2GB x32 route using old-generation Micron/Y52-series direction | S1/S2/S14/S15 | The old 2GB path conflicts with the 5-8 year lifecycle target due to EOL/PCN evidence and lack of a current long-life replacement. |
| Rejected | Samsung `K3KL8L80DM-TGCT` 245FBGA consumer route | S1/S2/S10 | Supplier feedback says current output product does not match capacity/lifecycle needs; consumer lifecycle is typically 2-3 years; package is 245FBGA, not a clean substitute for the Micron 315-ball path. |
| Rejected | Nanya route | S1/S2/S11 | Supplier feedback says Nanya has no LPDDR5. |
| Watchlist | Samsung 315FBGA public-candidate direction: `K3KL8L80QM-MFCT`, `K3KL8L80CM-MGCT`, and related 32Gb x32 parts | S16/S17 | Useful as a second-source investigation path, but current evidence is a project note based on public information, not formal supplier confirmation. Keep parallel procurement active, but do not treat these as backup yet. |
| Watchlist | Henry / HSRP or other Hynix channel | S1/S2/S12/S17 | Procurement request exists, but no reply was found in the searched Gmail range. Cannot count as a candidate until a formal response arrives. |

## Evidence Matrix

| Field | Candidate | Requirement | Claimed value | Evidence source | Evidence date | Status | Notes |
|---|---|---|---|---|---|---|---|
| Interface / protocol | Micron `MT62F1G32D2DS-020 WT:D` | LPDDR5 preferred; LPDDR5X acceptable only after compatibility and tool validation | LPDDR5X SDRAM with LPDDR5X/LPDDR5 data interface | S13 via S1 | 2026-03 / 2026-05-08 extract | confirmed | Confirms it is a credible LPDDR5X evaluation candidate, not a pure LPDDR5 part. |
| Width | Micron `MT62F1G32D2DS-020 WT:D` | x32 per component | x32 | S8/S13 via S1/S2 | 2026-05-08 | confirmed | Meets the x32 architecture assumption. |
| Capacity | Micron `MT62F1G32D2DS-020 WT:D` | Original 2GB / 16Gb; changeable only by owner approval | 4GB / 32Gb | S8/S13 via S1/S2 | 2026-05-08 | conflict | This is the main requirement change: 2 components become 8GB total instead of the planned 4GB total. |
| Speed rating | Micron `MT62F1G32D2DS-020 WT:D` | Run at 3733 Mbps/pin on Agilex 5 target | 9600 Mb/s per pin part | S9/S13 via S1/S2 | 2026-05-08 | TBD-evidence | High-speed part can be evaluated for lower-speed use, but supplier guidance and Quartus closure are still missing. |
| Package | Micron `MT62F1G32D2DS-020 WT:D` | Standard BGA/package usable in DF108 layout | 315-ball TFBGA, package code DS | S13 via S1/S2 | 2026-03 / 2026-05-08 extract | confirmed | Package identity is known; DF108 footprint, escape, and SI feasibility are still not confirmed. |
| Temperature / grade | Micron `MT62F1G32D2DS-020 WT:D` | Commercial grade acceptable | `WT:D` appears in part number | S8/S13 via S1/S2 | 2026-05-08 | TBD-evidence | Meaning of `WT:D`, temperature range, and supply grade require formal Micron/WT/WPI confirmation. |
| Lifecycle / EOL / PCN | Micron `MT62F1G32D2DS-020 WT:D` | 5-8 year no known EOL risk | Supplier says Micron is pushing 9600 MT/s direction; exact Y62P lifecycle not formally confirmed | S8/S9/S13 via S1/S2 | 2026-05-08 | TBD-evidence | PCN evidence rejects old routes but does not prove long-life status for this exact Y62P part. |
| Commercial terms | Micron `MT62F1G32D2DS-020 WT:D` | Price, MOQ/MPQ, sample lead, MP lead acceptable | Not provided | S3 | 2026-05-08 | TBD-evidence | Procurement must request and record formal terms. |
| Toolchain support | Micron `MT62F1G32D2DS-020 WT:D` | Quartus EMIF + Pin Planner + Fitter pass on exact target | No tool report yet | S1/S4/S5/S6/S7 | 2026-05-08 | TBD-evidence | Required before pin-list freeze. |
| Resource coexistence | Micron `MT62F1G32D2DS-020 WT:D` | `MIPI + 2x LPDDR5 x32 + 168 adjustable GPIO` closes on B32A target | Not proven | S5/S6/S7 | 2026-05-07 to 2026-05-08 | TBD-evidence | This is a P0 architecture/resource blocker, not just a memory-part issue. |
| Lifecycle / EOL / PCN | Old 2GB x32 route | 5-8 year no known EOL risk | Y52P/Y52Q-related old routes have EOL/PCN risk | S14/S15 via S1/S2 | 2026-02-04 / 2026-04-22 | conflict | Do not freeze an old 2GB route without a new non-EOL formal replacement. |
| Width / capacity | Samsung `K3KL8L80DM-TGCT` | x32, originally 2GB preferred | 32Gb / 4GB, x32 | S10 via S1/S2 | 2026-05-08 | conflict | Width is usable, capacity is same 4GB-change issue as Micron. |
| Package | Samsung `K3KL8L80DM-TGCT` | Package usable as project path | 245FBGA, 8.2 x 12.4 mm | S10 via S1/S2 | 2026-05-08 | conflict | Package differs from 315-ball direction and cannot be assumed substitute-compatible. |
| Lifecycle | Samsung `K3KL8L80DM-TGCT` | 5-8 year no known EOL risk | Supplier states consumer lifecycle usually 2-3 years | S10 via S1/S2 | 2026-05-08 | conflict | Reject as main path. |
| Watchlist source | Samsung 315FBGA public-candidate direction | Formal supplier evidence required | Public/project-note candidates include 32Gb x32 315FBGA parts | S16/S17 | 2026-05-08 | TBD-evidence | Keep in procurement watchlist; do not mark backup until formal quote/lifecycle evidence exists. |
| Availability | Nanya route | LPDDR5 source available | Nanya has no LPDDR5 | S11 via S1/S2 | 2026-05-08 | conflict | Route closed. |
| Availability | Henry / HSRP / Hynix channel | Formal candidate or rejection needed | Request sent; no reply in searched range | S12 via S1/S2 | 2026-05-08 | TBD-evidence | Follow-up channel only. |

## Evidence Gaps

P0 gaps before schematic/BOM/pin freeze:

- Formal supplier confirmation for Micron `MT62F1G32D2DS-020 WT:D`: lifecycle, PCN/EOL posture, exact temperature/supply grade for `WT:D`, sample lead time, production lead time, price ladder, MOQ, and MPQ.
- Formal statement from Micron/WT/WPI on using the 9600 Mb/s part at the DF108 target of 3733 Mbps/pin, including any initialization, ODT, training, SI, or validation caveats.
- Project owner approval that the memory capacity changes from planned 2 x 2GB = 4GB total to 2 x 4GB = 8GB total.
- Quartus exact-device proof for the final target: EMIF config/export, Pin Planner output, Fitter report, QSF/pin report, and explicit resource-conflict statement.
- P0 resource proof that the final B32A device can fit `MIPI + 2x LPDDR5 x32 + 168 adjustable GPIO`. If not, the architecture must change before any LPDDR5 package/pin freeze.
- Hardware package proof for the Micron 315-ball TFBGA DS path: symbol, footprint, escape feasibility, power rails, RZQ, reset, refclk, ODT/termination, VREF-related handling, and SI/PI constraints.

P1 gaps to improve supply resilience:

- Formal Samsung 315FBGA channel confirmation for `K3KL8L80QM-MFCT`, `K3KL8L80CM-MGCT`, or another long-life 32Gb x32 candidate.
- Henry/HSRP or Hynix response confirming whether a 2GB x32 long-life part exists, or whether only 4GB x32 parts are realistic.
- Explicit bring-up strategy: lower FSP values for initial board bring-up before target 3733 Mbps/pin.
- Software/firmware impact assessment for 8GB total memory: address map, memory test, boot/init, calibration, and any licensing/cost side effects.

## Risk Register

| Category | Description | Probability | Impact | Mitigation action | Owner | Review date |
|---|---|---|---|---|---|---|
| Supply / allocation / lead time | Micron primary has no recorded sample/MP lead time, allocation statement, MOQ, MPQ, or price yet. | M | H | Procurement sends the S3 question list to WT/WPI/Micron and records formal response against this decision. | Procurement | 2026-05-13 |
| Lifecycle / EOL / PCN | Exact Y62P Micron primary is not formally proven to meet the 5-8 year target; old 2GB routes already show EOL risk. | M | H | Require lifecycle/PCN/EOL posture for the exact part number; do not use old 2GB routes unless a non-EOL replacement is formally identified. | Procurement + project owner | 2026-05-13 |
| Package / pinout / footprint | 315-ball TFBGA DS package is known, but DF108 symbol, footprint, escape, and pinout legality are not proven. | M | H | Build preliminary symbol/footprint only after Quartus pin planning; archive package drawing and pinout evidence with the schematic library review. | Hardware | 2026-05-14 |
| SI / PI / thermal / mechanical | 9600-rated LPDDR5X part derated to 3733 Mbps/pin still needs ODT/training/SI/power validation; 8GB capacity may affect power and thermal. | M | H | Request supplier derating guidance; run board-level SI/PI precheck after pin plan; update power estimate for 2 x 4GB devices. | Hardware + logic | 2026-05-15 |
| Firmware / logic / toolchain | No Quartus EMIF, Pin Planner, or Fitter artifact exists for two x32 LPDDR5 groups on the exact target. | H | H | Logic owner creates a minimal Quartus project using the final device/package/speed grade and exports EMIF, QSF, pin, and Fitter results. | Logic / 吴志安 | 2026-05-12 |
| Cost / MOQ / MPQ / commercial terms | Capacity increases from 4GB total to 8GB total and may increase BOM cost; commercial terms are unknown. | H | M | Project owner decides whether 8GB is acceptable; procurement obtains pricing ladder and MOQ/MPQ before BOM freeze. | Project owner / 罗奇军 + procurement | 2026-05-13 |
| Substitute / second-source path | No confirmed backup candidate exists; Samsung 315FBGA route is only watchlist, and Henry/Hynix has no reply yet. | M | H | Run Micron and Samsung 315FBGA formal inquiries in parallel; keep Henry/Hynix follow-up open; record explicit no-second-source risk if unresolved. | Procurement | 2026-05-15 |
| Architecture / resource closure | A5ED B32A may not have enough HSIO resources for MIPI, 2 x x32 LPDDR5, and 168 adjustable GPIO together. | H | H | Quartus resource closure must include memory, MIPI, and all adjustable GPIO at the same time; if it fails, decide between different device/package, fewer GPIO, external expander/CPLD, or memory topology change. | Logic + hardware + project owner | 2026-05-12 |
| Requirement control | The original 2GB-per-component requirement is currently contradicted by all viable candidates. | H | H | Convert the capacity change into a formal requirement update or block memory selection from freeze. | Project owner | 2026-05-13 |

## Engineering Verification Gates

| Gate | Owner | Pass criteria | Artifact / link | Status |
|---|---|---|---|---|
| Requirement change gate | Project owner / 罗奇军 | Written approval that 2 x 4GB x32, 8GB total is acceptable for BOM cost, software address map, initialization, power, and thermal budget. | Requirement update or signed project note | blocked |
| Supplier evidence gate | Procurement | Formal reply for exact Micron part: lifecycle, PCN/EOL posture, `WT:D` grade, sample lead, MP lead, price ladder, MOQ, MPQ, and 3733 Mbps/pin derating guidance. | Supplier email / vendor quote / vendor PCN docs | TBD-evidence |
| Quartus EMIF gate | Logic / 吴志安 | Exact target device/package/speed grade configured with two x32 LPDDR5/LPDDR5X groups at target 3733 Mbps/pin; EMIF parameters exportable without unsupported configuration. | EMIF config screenshot/export | TBD-evidence |
| Pin Planner and Fitter gate | Logic / 吴志安 | Pin Planner and Fitter pass or produce an explicit conflict list for `MIPI + 2x LPDDR5 x32 + 168 adjustable GPIO`. | Pin Planner output, Fitter report, QSF/pin report | TBD-evidence |
| Package/library gate | Hardware | Micron 315-ball TFBGA DS symbol and footprint reviewed against datasheet/package drawing; no library mismatch remains. | Schematic library review and footprint check | TBD-evidence |
| Power and reference gate | Hardware | Rails, reset, RZQ/ZQ, refclk, ODT/termination, VREF-related handling, sequencing, and decoupling plan are checked against vendor and EMIF requirements. | Power/interface checklist | TBD-evidence |
| SI/PI/layout feasibility gate | Hardware | Preliminary escape, layer/impedance/length-match strategy, SI/PI assumptions, and board-space feasibility are acceptable for target speed and package. | Layout/SI precheck | TBD-evidence |
| Second-source gate | Procurement + project owner | Either a credible backup/watchlist path is formally recorded, or the project owner explicitly accepts single-source risk with mitigation. | Samsung/Micron/Hynix supplier record or risk acceptance | TBD-evidence |
| Bring-up strategy gate | Logic + hardware | Lower-speed FSP bring-up plan exists before attempting target rate. | Bring-up plan | TBD-evidence |

## Recommendation

Decision strength: selected-not-frozen.

Proceed with Micron `MT62F1G32D2DS-020 WT:D` as the primary candidate for procurement confirmation and engineering validation.

Do not freeze schematic, BOM, pin list, package footprint, or PCB constraints yet.

The current best engineering path is:

- Treat the original 2GB x32 requirement as commercially and lifecycle-risky unless a new formal supplier response proves otherwise.
- Use the Micron 4GB x32 LPDDR5X 315-ball path as the main validation path because it is the only concrete first-tier candidate with usable part-number and datasheet evidence.
- Keep Samsung 315FBGA 32Gb x32 parts in watchlist as a potential second-source path, but do not call them backup until formal supplier evidence exists.
- Reject the Samsung 245FBGA consumer route, Nanya route, and old 2GB EOL-prone route for the current freeze path.
- Make the P0 resource closure explicit: the memory part decision is blocked from freeze until Quartus proves the complete final system placement, not just a standalone memory controller.

## Freeze Checklist

| Gate | Required evidence | Owner | Status | Notes |
|---|---|---|---|---|
| Requirement baseline approved | Requirement record with hard/changeable constraints | Project owner | blocked | Original baseline exists, but 4GB-per-component capacity change is not approved. |
| Primary candidate selected | Decision record with Primary/Backup/Rejected/Watchlist | Hardware + procurement | pass | Micron selected as primary for validation only. |
| Vendor evidence reconciled | Datasheet, PCN/EOL, supplier response, or official URL | Procurement | blocked | Datasheet extract exists; lifecycle, grade, derating, and commercial evidence still missing. |
| Lifecycle and PCN window acceptable | PCN/EOL evidence and project lifetime criterion | Procurement | TBD-evidence | Old routes are risky; exact Micron Y62P long-life status is not formally confirmed. |
| Commercial terms acceptable | Price, MOQ/MPQ, sample and production lead time | Procurement | TBD-evidence | No formal terms recorded. |
| Toolchain or engineering validation passed | Tool report, simulation, lab result, or review artifact | Logic | TBD-evidence | No Quartus artifacts yet. |
| Package / footprint / pinout checked | Library, pinout, layout, or mechanical evidence | Hardware | TBD-evidence | Package known; DF108 implementation not checked. |
| SI / PI / thermal / mechanical constraints checked | Decision-specific validation artifact | Hardware | TBD-evidence | Derating, escape, SI/PI, and power not closed. |
| Firmware / logic / software impact accepted | Owner signoff or linked change record | Logic + software + project owner | TBD-evidence | 8GB total impact and initialization plan not accepted. |
| Substitute or mitigation path recorded | Backup candidate or explicit risk acceptance | Procurement + project owner | blocked | No confirmed backup; Samsung 315FBGA remains watchlist. |
| Open risks have owners and review dates | Risk register | Hardware | pass | This record assigns owners and dates. |
| Project record location created | Saved decision artifact and index pointer | Hardware | pass | This file is the project decision artifact. Workspace index pointer has been added in `/home/ubuntu/workspace/CONTEXT_INDEX.md`. |

Freeze recommendation: blocked for freeze, selected-not-frozen for validation.

## Record Location

Saved project record:

`/home/ubuntu/hardware-projects/prj/DF108/revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/05_decisions/20260508-lpddr5-selection.md`

Related selection map:

`/home/ubuntu/hardware-projects/prj/DF108/revisions/rev-20260506-df108-ku040-to-a5ed052ab32ae2v/05_decisions/20260508-lpddr5-selection-map.md`

Workspace index pointer:

`CONTEXT_INDEX.md` -> A38 / DF108 / Agilex 5 -> LPDDR5 selection decision.

## Next Actions

P0, by 2026-05-12 to 2026-05-13:

| Owner | Action | Output |
|---|---|---|
| Project owner / 罗奇军 | Decide whether 8GB total memory is acceptable when replacing the planned 2 x 2GB x32 parts with 2 x 4GB x32 parts. | Requirement-change approval or rejection. |
| Procurement | Send S3 Micron/WT/WPI questions for exact part `MT62F1G32D2DS-020 WT:D`: lifecycle, `WT:D` grade, lead time, price, MOQ/MPQ, 2GB alternative, derating guidance. | Formal supplier reply archived with message date and sender. |
| Logic / 吴志安 | Build minimal Quartus project for final target device/package/speed grade, two x32 LPDDR5/LPDDR5X groups at 3733 Mbps/pin, and coexistence with MIPI plus 168 adjustable GPIO. | EMIF export, Pin Planner output, Fitter report, QSF/pin report, conflict statement. |
| Hardware | Prepare preliminary Micron 315-ball DS package/library feasibility review, but do not freeze pin list. | Symbol/footprint feasibility note and implementation blockers. |
| Procurement | Ask Samsung formal channels for 32Gb x32 315FBGA lifecycle/commercial evidence, especially `K3KL8L80QM-MFCT` and `K3KL8L80CM-MGCT` if available. | Watchlist update: promoted to Backup only if evidence is formal and passes gates. |
| Procurement | Follow Henry/HSRP/Hynix channel once. | Reply or explicit no-response status. |

Decision review trigger:

- If Quartus cannot place `MIPI + 2x LPDDR5 x32 + 168 adjustable GPIO`, reopen architecture before further LPDDR5 component work.
- If Micron cannot confirm lifecycle/commercial/derating, keep Micron as watchlist only and promote a formally evidenced alternative if one exists.
- If project owner rejects 8GB total memory, the current primary becomes blocked and procurement must restart around 2GB x32 or a different memory topology.
