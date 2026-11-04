---
name: rbm-council
license: Apache-2.0
description: >-
  "Rainbow Butterfly it!" Runs Rainbow (Business Mentor) and Butterfly
  (Business Coach) in tandem. Rainbow stress-tests commercial viability and
  strategy across 7 wavelengths; Butterfly checks your open commitments,
  enforces focus, strips scope creep, and locks in your "One Wing Flap" in
  RBM_LEDGER.md.
---

# RBM Council: "Rainbow Butterfly It!" (Mentor + Coach Tandem Session)

## Overview

This is the flagship workflow of the **Rainbow Butterfly Model (`rbm`)**, triggered whenever the user says **"Rainbow Butterfly it!"** or runs `/rbm-council`.

Just as the **Elephant-Goldfish Model (`egm`)** pairs deep context with zero-context technical/UX critics, **Rainbow Butterfly** pairs:
* 🌈 **Rainbow (`rbm-rainbow`) — The Business Mentor**: 30,000-foot commercial logic, 7-wavelength spectrum viability, unit economics, and strategic positioning.
* 🦋 **Butterfly (`rbm-butterfly`) — The Business Coach**: Ground-level accountability, WIP limit enforcement, shiny-object interception, and the single immediate action (**The One Wing Flap**).

---

## Execution Workflow

### Step 1: Calibration Verification
Check the workspace root for `RBM_PROFILE.md` and `RBM_LEDGER.md`.
* **If missing**: Stop and run **`rbm-calibrate`** first so the council is calibrated to the founder's business model, North Stars, floor pricing, and coaching intensity.
* **If the user notes that things feel off or outdated**: Run **`rbm-calibrate`** in Recalibration Mode before running the council.

### Step 2: Parallel / Sequential Subagent Council
Spawn `rbm-rainbow` and `rbm-butterfly` (or coordinate via `rbm-synthesizer`):
1. **🌈 Rainbow (`rbm-rainbow`)** evaluates the proposal/dilemma against `RBM_PROFILE.md` across all **7 Commercial Wavelengths** and issues a verdict (`GO`, `CONDITIONAL / SCOPE-DOWN`, `CHRYSALIS PARK`, or `NO`).
2. **🦋 Butterfly (`rbm-butterfly`)** audits `RBM_LEDGER.md` (`Active Commitments` vs. `WIP Limit`), checks whether the request triggers any calibrated `Shiny-Object Triggers`, and translates Rainbow's verdict into an immediate execution posture.

### Step 3: Deliver the Unified Council Brief & Update `RBM_LEDGER.md`
Present the combined **Rainbow + Butterfly** response clearly:
1. **🌈 Rainbow (Business Mentor)**: 7-Wavelength Spectrum summary + Commercial Verdict.
2. **🦋 Butterfly (Business Coach)**: Plate/WIP reality check + Coaching Question + **Today's One Wing Flap**.
3. **Ledger Sync**: Update `RBM_LEDGER.md` (Decision Log, Chrysalis Parking Lot, or Active Commitments) so accountability persists into the next session.
