---
name: rbm-mentor
license: Apache-2.0
description: >-
  Calls on Rainbow (rbm-rainbow), your calibrated Business Mentor. Evaluates
  any business idea, offer, pricing structure, client proposal, or product
  decision across the 7-Wavelength Commercial Spectrum and logs the decision
  in RBM_LEDGER.md.
---

# RBM Mentor: Call on Rainbow (Business Mentor)

## Overview

Use this skill when the user wants **business expert eyes and commercial logic** on an idea, offer, pricing model, client deal, or roadmap choice (`"Call Rainbow"`, `"Ask my business mentor"`, `"/rbm-mentor"`).

## Workflow

1. **Calibration Pre-Check**:
   * Check for `RBM_PROFILE.md` and `RBM_LEDGER.md` in the workspace root.
   * If `RBM_PROFILE.md` is missing, stop and run `rbm-calibrate` first so Rainbow knows the founder's business model, North Stars, and floor pricing.
2. **Spawn Rainbow Subagent**:
   * Invoke the `rbm-rainbow` subagent (`agents/rainbow_mentor.md`) with the user's question/proposal and the paths to `RBM_PROFILE.md` and `RBM_LEDGER.md`.
   * If running in an environment without subagent spawning, adopt `agents/rainbow_mentor.md` directly in a fresh analytical pass.
3. **Present the 7-Wavelength Spectrum Audit**:
   * Deliver Rainbow's commercial breakdown (Market/Buyer Urgency, Unit Economics, Portfolio Fit, Asset Leverage, Opportunity Cost, Risk/Moat, 6–36 Month Scale Path) and explicit verdict (`GO`, `CONDITIONAL / SCOPE-DOWN`, `CHRYSALIS PARK`, or `NO`).
4. **Update the Decision Log**:
   * Once the user confirms their decision, record the verdict and commercial rationale in Section 3 (`Rainbow Decision Log`) or Section 4 (`Chrysalis Parking Lot`) of `RBM_LEDGER.md`.
