---
name: rbm-coach
license: Apache-2.0
description: >-
  Calls on Butterfly (rbm-butterfly), your calibrated Business Coach. Runs
  daily/weekly focus check-ins, audits open commitments in RBM_LEDGER.md,
  catches shiny-object procrastination, enforces your WIP limit, and defines
  today's single highest-leverage action ("The One Wing Flap").
---

# RBM Coach: Call on Butterfly (Business Coach)

## Overview

Use this skill when the user needs **accountability, focus protection, momentum, or a check-in** (`"Call Butterfly"`, `"Coach me"`, `"Check my plate"`, `"I'm feeling scattered"`, `"/rbm-coach"`).

## Workflow

1. **Calibration Pre-Check**:
   * Check for `RBM_PROFILE.md` and `RBM_LEDGER.md` in the workspace root.
   * If `RBM_PROFILE.md` is missing, run `rbm-calibrate` first.
2. **Reality & Workspace Inspection**:
   * Read `RBM_PROFILE.md` (to check `Coaching Intensity Level`, `WIP Limit`, and `Shiny-Object Triggers`) and `RBM_LEDGER.md` (to check `Active Commitments` and `Today's One Wing Flap`).
   * Optionally check recent git commits or modified files in the workspace to see whether active commitments have tangible progress.
3. **Spawn Butterfly Subagent**:
   * Invoke `rbm-butterfly` (`agents/butterfly_coach.md`) with the current ledger state and the user's prompt.
4. **Update `RBM_LEDGER.md`**:
   * Mark any shipped items as completed (moving them to Section 5 `Completed Flights`).
   * Park any distractions in Section 4 (`Chrysalis Parking Lot`).
   * Write the agreed **One Wing Flap** and its Definition of Done into Section 2 of `RBM_LEDGER.md`.
