# Current Design Direction For External LLM

This file is a concise handoff update for another LLM. It summarizes the latest 2026-05-07 design direction.

It is not schematic sign-off, board-release approval, or a formal design baseline.

## Latest User Inputs

1. Remove the HS/LP switching circuit and remove the buffer. MIPI comes from the decoder board, passes through the connector, and connects directly to the Agilex 5 device.
2. Connect all MIPI lanes to `A5EC052A B32A` HSIO banks.
3. Replace DDR4 with LPDDR5.
4. Use the mature LM5060 input-power circuit and migrate it to this revision.

## Current Technical Position

### MIPI

Recommended topology:

```text
Decoder board MIPI D-PHY
  -> board-to-board connector
  -> controlled-impedance routing
  -> A5EC052A B32A MIPI-capable HSIO bank
  -> Agilex 5 MIPI D-PHY IP
```

Interpretation:

- Removing the HS/LP switch and buffer is directionally correct if the decoder board really outputs a standard MIPI D-PHY interface.
- Do not treat this as a generic differential IO connection.
- Use Agilex 5 MIPI D-PHY IP placement rules, RZQ/refclk rules, and MIPI-capable HSIO banks.
- For Agilex 5 E-Series Group A, use these rate boundaries:
  - short/standard channel: up to `3.5 Gbps/lane`
  - long/lossy channel: design around `2.5 Gbps/lane`

### LPDDR5

For the current `A5EC052A B32A` placeholder / Agilex 5 E-Series Group A interpretation:

| Item | Design value |
|---|---:|
| LPDDR5 clock | `1,866.667 MHz` |
| LPDDR5 data rate | `3,733 Mbps/pin` |
| x16 raw bandwidth | about `7.46 GB/s` |
| x32 raw bandwidth | about `14.93 GB/s` |

Do not assume that higher EMIF parameter choices are valid for this exact device/package/speed grade. Confirm with Quartus EMIF IP, pin planner, final Intel/Altera documentation, and the selected LPDDR5 vendor datasheet.

Recommended memory candidates:

- LPDDR5 `x32`
- LPDDR5 `2ch x16`

The schematic should be planned so that LPDDR5 EMIF banks, byte lanes, RZQ, refclk, address/command lanes, and data lanes are legal before symbols are wired.

### LM5060

The LM5060 front-end can be migrated as a mature input-power block.

Still re-check:

- UV/OV thresholds
- current limit and sense resistor
- hot-swap MOSFET SOA
- inrush and downstream bulk capacitance
- TVS/fuse/EMI protection
- `PG` / `FLT` handoff into the new Agilex 5 power sequencing

## Decision-Level Summary

The recommended main architecture is:

```text
DF108 preserved external domain
  -> decoder board MIPI output
  -> connector
  -> direct MIPI routing
  -> A5EC052A B32A MIPI-capable HSIO banks

DC24V input
  -> migrated LM5060 protection/hot-swap block
  -> new Agilex 5 + LPDDR5 power tree

External memory
  -> LPDDR5 hard memory controller
  -> target design capability 3,733 Mbps/pin
```

The next required artifact is an `A5EC052A B32A resource allocation matrix` covering MIPI lanes, LPDDR5 EMIF banks, power sequencing, clock/reset dependencies, and final A5EC/A5ED naming cleanup.

## Source Files Used

User reference folder:

- `https://drive.google.com/drive/folders/1LBmcH09JFtY-A9iW-TYNtksNjdZ7o8wS?dmr=1&ec=wgc-drive-%5Bmodule%5D-goto`

Downloaded reference files used for this update:

- `Agilex 5 FPGAs and SoCs Device Overview ug-762191-762192.pdf`
- `Agilex 5 FPGAs and SoCs Device Data Sheet-ds-813918-813919.pdf`
- `External Memory Interfaces (EMIF) IP User Guide Agilex 5 FPGAs and SoCs 817467_D842785.pdf`
- `General-Purpose IO User Guide Agilex 5 FPGAs and SoCs 813934_869633.pdf`
- `MIPI D-PHY IP User Guide 817561_856924.pdf`
- `altera-pbc-b32a-a5e.xlsx`

Use the longer evidence note for engineering details:

- `../02_design_evidence/current_design_direction_20260507.md`
