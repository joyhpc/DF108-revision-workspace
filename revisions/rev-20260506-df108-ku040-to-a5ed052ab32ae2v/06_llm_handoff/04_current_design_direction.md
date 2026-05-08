# Current Design Direction For External LLM

This file is a concise handoff update for another LLM. It summarizes the latest 2026-05-07 design direction.

It is not schematic sign-off, board-release approval, or a formal design baseline.

## Latest User Inputs

1. Remove the HS/LP switching circuit and remove the buffer. MIPI comes from the decoder board, passes through the connector, and connects directly to the Agilex 5 device.
2. Connect all MIPI lanes to `A5EC052A B32A` HSIO banks.
3. Replace DDR4 with LPDDR5.
4. Use the mature LM5060 input-power circuit and migrate it to this revision.
5. Completely delete the old `KU040` path in the target Rev1 schematic.
6. Allocate 168 ordinary decoder-board GPIO signals to adjustable `1.2 V` to `1.8 V` I/O banks.

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
| Rev1 topology | 2 x `x32` LPDDR5 component groups |
| Controller allocation | one LPDDR5 hard memory controller per group |

Do not assume that higher EMIF parameter choices are valid for this exact device/package/speed grade. Confirm with Quartus EMIF IP, pin planner, final Intel/Altera documentation, and the selected LPDDR5 vendor datasheet.

The Rev1 schematic should be planned as `LPDDR5_CTRL0_X32` and `LPDDR5_CTRL1_X32`. Each group owns one x32 component resource domain and one hard memory controller. LPDDR5 EMIF banks, byte lanes, RZQ, refclk, address/command lanes, and data lanes must be proven legal before symbols are wired.

### LM5060

The LM5060 front-end can be migrated as a mature input-power block.

Still re-check:

- UV/OV thresholds
- current limit and sense resistor
- hot-swap MOSFET SOA
- inrush and downstream bulk capacitance
- TVS/fuse/EMI protection
- `PG` / `FLT` handoff into the new Agilex 5 power sequencing

### KU040 Removal And Decoder GPIO

Target Rev1 should not keep `U14=XCKU040-2FFVA1156I` as a dual-option controller. Old KU040-owned interfaces must be deleted or reassigned to Agilex 5, MCU, decoder board, or preserved peripheral logic.

The 168 ordinary decoder-board GPIO signals should be planned as four logical groups:

| Group | Count | Target |
|---|---:|---|
| `DEC_GPIO_VADJ_G0` | 42 | one HSIO / `VCCIO_PIO` sub-bank |
| `DEC_GPIO_VADJ_G1` | 42 | one HSIO / `VCCIO_PIO` sub-bank |
| `DEC_GPIO_VADJ_G2` | 42 | one HSIO / `VCCIO_PIO` sub-bank |
| `DEC_GPIO_VADJ_G3` | 42 | one HSIO / `VCCIO_PIO` sub-bank |

Use HSIO / `VCCIO_PIO` for `1.2 V` to `1.8 V` adjustable GPIO. Do not assign these signals to exact balls until Quartus Pin Planner confirms the same device can also fit MIPI and both LPDDR5 x32 controller groups.

Important capacity warning: local pinout evidence shows `A5EC052A_B32A` has 8 HSIO sub-banks, while `A5ED052A_B32A` has 4. If final A5ED only exposes four HSIO sub-banks, 168 GPIO consumes nearly all adjustable HSIO capacity before MIPI and LPDDR5 are placed.

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
  -> 2 groups of x32 LPDDR5 components
  -> one controller per group
  -> target design capability 3,733 Mbps/pin

Ordinary decoder GPIO
  -> 168 signals
  -> 4 groups of 42
  -> HSIO / VCCIO_PIO adjustable banks
  -> exact bank/pin pending Quartus Pin Planner
```

The current required artifact is `../02_design_evidence/a5ec052a_b32a_resource_allocation_matrix_20260507.csv`, covering MIPI lanes, LPDDR5 EMIF banks, power sequencing, clock/reset dependencies, and final A5EC/A5ED naming cleanup.

GPIO/KU040 deletion evidence:

- `../02_design_evidence/ku040_removal_gpio_bank_allocation_20260508.md`

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
