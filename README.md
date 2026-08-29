# CFM56-5B Turbofan Engine — CAD Model

Full SolidWorks model of a high-bypass turbofan, built proportionally around the CFM International CFM56-5B (Airbus A320 family). A self-directed summer project to rebuild CAD fluency and understand real turbofan architecture beyond coursework.

## Overview

Built over roughly 48-72 hours as a single multi-body part with 176 features, modelling a simplified alternating rotor/stator axial architecture. The fan matches the real CFM56-5B blade count exactly (36 blades); the LPC and HPC stage counts were simplified relative to the real engine (4-stage LPC and 9-stage HPC) to keep build scope manageable, while preserving the real architecture pattern (alternating rotor/stator, tip shrouds, variable stator vanes).

| Section | Rotor blade stages | Stator vane stages |
|---|---|---|
| Fan | 36 | — |
| LPC | 3 (real engine: 4) | 3 |
| HPC | 6 (real engine: 9) | 7 |
| Combustor | — | — |
| HPT | 1 | 1 |
| LPT | 4 | 4 |

## Key technical features

- **LPC variable stator vanes**: modelled with an actuation linkage reflecting the real mechanism used to prevent compressor stall at low engine speeds.
- **LPT tip shrouds**: modelled on each rotor stage based on labyrinth seal design, used in real turbines to minimise gas leakage around blade tips.
- **Fan and compressor blades**: built as twisted, tapered aerofoils using a NACA 65(1)-412 profile, lofted across root, mid-span, and tip sections to capture true blade geometry.

## Techniques applied

- Circular patterning across multi-stage geometry
- Guide-curve lofts for twisted blade profiles
- Multi-body part management along a shared axis
- Troubleshooting SolidWorks rebuild errors on tightly packed, high-blade-count stages (geometry pattern limitations, zero-thickness geometry)

## Scope and assumptions

This is a static geometric representation, not a functional mechanism. Overall proportions (fan diameter, engine length) are based on published CFM56-5B specifications, and the fan blade count (36) matches the real engine exactly. LPC and HPC stage counts were deliberately simplified relative to the real engine (see table above) to keep build scope manageable within the project timeframe; the alternating rotor/stator pattern, variable stator vane mechanism, and turbine tip shrouds were modelled to reflect real engine architecture regardless of the simplified stage count. Dimensions not publicly available were estimated proportionally from the engine's own technical diagrams.

## Repository structure

```
/solidworks/
  CFM56_5B_Turbofan.SLDPRT — full multi-body part
/images/
  assembled_view_fan_casing.png
  internal_section_full_stage_sequence.png
```

## Author

Mohaned Elkurdi — MEng Aerospace Engineering, University of Manchester
