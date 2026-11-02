# Hackpad by kr4phy
This is my hackpad design.
This pad contains one rotary encoder (including a switch), 8 keys (4*2 matrix), and an OLED screen and uses all GPIO pins.

## Overview
- 8 macro key matrix (4*2)
- Rotary encoder knob with switch
- 0.96" OLED display
- XIAO RP2040 mcu

## Project structure
```
hackpad/
├── LICENSE
├── README.md
│
├── Rotary_Encoder.pretty/            # KiCad encoder footprints
│
├── case/                            # 3d models for case
│   ├── hackpad.f3d                  # Fusion 360 project file
│   ├── hackpad.step                 # STEP model file
│   ├── hackpad_ap242.step            # STEP AP242 file
│   ├── plate-2026-10-29T14_19_29.061Z.dxf
│   └── plate-2026-11-01T02_40_03.895Z.dxf
│
├── kicad_care_package/
│   ├── SK6812MINI-E.kicad_sym
│   ├── XIAO_RP2040.kicad_sym
│   └── footprints.pretty/
│       ├── SK6812MINI-E_fixed.kicad_mod
│       └── XIAO-Generic-Hybrid-14P-2.54-21X17.8MM.kicad_mod
│
└── pcb/                             # Files about PCB design
    ├── DRC.rpt                      # Design Rule Check report
    ├── fp-lib-table
    ├── hackpad.dsn
    ├── hackpad.kicad_pcb
    ├── hackpad.kicad_prl
    ├── hackpad.kicad_pro
    ├── hackpad.kicad_sch
    ├── hackpad.ses
    ├── hackpad_auto_routed.dsn
    ├── sym-lib-table
    ├── sym-lib-table.bak
    └── ~hackpad.kicad_pro.lck
```

## Firmware
Firmware is under development. Not implemented yet, but I planned to make it possible to customize the keymap using only the pad without an external PC. I also planned to create a menu that can be operated with a rotary encoder.

