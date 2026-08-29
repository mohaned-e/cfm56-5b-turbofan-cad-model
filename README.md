# CFM56-5B Turbofan Engine — CAD Model

Full SolidWorks model of a high-bypass turbofan, built proportionally around the CFM International CFM56-5B (Airbus A320 family). A self-directed summer project to rebuild CAD fluency and understand real turbofan architecture beyond coursework.

## Overview

Built over roughly 48–72 hours as a single multi-body part with 176 features, modelling all major engine sections in sequence:

- 22-blade fan
- Low-pressure compressor (LPC)
- High-pressure compressor (HPC)
- Annular combustor
- High-pressure turbine (HPT)
- 4-stage low-pressure turbine (LPT)

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

This is a **static geometric representation**, not a functional mechanism. Overall proportions (fan diameter, engine length) are based on published CFM56-5B specifications. Individual stage counts and dimensions not publicly available were estimated proportionally from the engine's own technical diagrams and cross-referenced against real compressor/turbine design principles where possible.

## Repository structure

/solidworks/
    CFM56_5B_Turbofan.SLDPRT      — full multi-body part
/images/
    assembled_view_fan_casing.png
    internal_section_full_stage_sequence.png

## Author

Mohaned Elkurdi — MEng Aerospace Engineering, University of Manchester
