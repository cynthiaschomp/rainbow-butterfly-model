---
name: rbm-calibrate
license: Apache-2.0
description: >-
  Initializes or recalibrates the Rainbow Butterfly Model (RBM) for the user's
  business. Creates or updates RBM_PROFILE.md (business model, North Stars,
  Rainbow mentor archetype, Butterfly coaching intensity, shiny-object triggers)
  and RBM_LEDGER.md (active commitments, WIP limit, decision log). Run this
  first after installing RBM, and run it again anytime priorities shift or
  mentorship/coaching feels off.
---

# RBM Calibrate: Setup & Recalibration Engine

## Overview

`rbm-calibrate` tunes **Rainbow** (Business Mentor) and **Butterfly** (Business Coach) to the founder's actual business architecture, revenue goals, unit-economics boundaries, shiny-object triggers, and preferred accountability style.

It supports two modes automatically:
1. **Initial Calibration (First Run)**: When `RBM_PROFILE.md` or `RBM_LEDGER.md` do not yet exist in the workspace.
2. **Recalibration Mode ("Things Feel Off")**: When `RBM_PROFILE.md` already exists, or when the user says *"recalibrate"*, *"things feel off"*, *"my priorities changed"*, or *"adjust Butterfly/Rainbow"*.

---

## Step 1: Detect Calibration State

Check the current workspace root for `RBM_PROFILE.md` and `RBM_LEDGER.md`.
* **If neither exists**: Announce **Initial Calibration Mode** and proceed to Step 2A.
* **If `RBM_PROFILE.md` exists**: Read both `RBM_PROFILE.md` and `RBM_LEDGER.md`, announce **Recalibration Mode**, and proceed to Step 2B.

---

## Step 2A: Initial Calibration Interview

Gather the 5 core calibration dimensions from the user. If you already know parts of their business context from the workspace (e.g., existing `AGENTS.md`, project directories, or user instructions), pre-populate what is verified and ask the user to confirm or fill in the rest using `ask_question` or concise direct questions:

1. **Business Architecture & Revenue Engines**:
   * What are your core business pillars/umbrellas and how does revenue enter (e.g., SaaS/plugin licenses, client retainers, fixed-scope builds, consulting)?
   * What is your verified baseline MRR/revenue (`--` if unconfigured), your 90-day target, and your floor price? *(Never guess financial figures.)*
2. **Current Season North Stars & Anti-Goals**:
   * What are the top 1–2 outcomes that matter most over the next 90 days?
   * What are your explicit **Anti-Goals** (what are we saying *NO* to right now)?
3. **Rainbow Mentor Tuning**:
   * Which Mentor Voice fits best?
     * `Board-Level Commercial Strategist` (Focus on enterprise value, moats, and portfolio leverage)
     * `Bootstrapped Unit-Economics Operator` (Focus on immediate cash flow, speed-to-revenue, and zero waste)
     * `Product-Led Growth Architect` (Focus on turning services into repeatable software/assets)
4. **Butterfly Coach Tuning**:
   * Which Coaching Intensity level do you want when new ideas compete with open commitments?
     * `Gentle Compass` (Supportive reminders and gentle realignment)
     * `Firm Momentum Partner` (Direct pushback on scope creep and clear timeboxing)
     * `Ruthless Gatekeeper` ("Finish your plate first" — blocks new side-quests until open commitments ship)
   * What is your maximum concurrent commitment limit (`WIP Limit`, default `3`)?
   * What are your classic **"Productive Procrastination" / Shiny-Object triggers**? *(e.g., spinning up a new tool/domain, refactoring CSS/code, over-researching before sending an offer)*
5. **Initial Plate (Top 1–3 Active Commitments)**:
   * What are the 1–3 active commitments on your plate this week, and what is today's **One Wing Flap**?

---

## Step 2B: Recalibration Mode ("When Things Feel Off")

When the user triggers recalibration, read `RBM_PROFILE.md` and `RBM_LEDGER.md` and run a **Calibration Drift Diagnostic**:

1. **Diagnose What Feels Off**: Ask the user (or evaluate from their prompt) which of the 4 drift patterns is happening:
   * **A. Strategic Drift**: Your North Stars or business season changed, so Rainbow is judging ideas against outdated goals.
   * **B. Tone / Pushback Mismatch**: Rainbow is too harsh or too lenient, or Butterfly's accountability intensity (`Gentle Compass` vs. `Firm Momentum Partner` vs. `Ruthless Gatekeeper`) needs dialing up or down.
   * **C. Plate Overload (Ledger Bankruptcy)**: `RBM_LEDGER.md` has accumulated stale commitments that are causing guilt rather than momentum.
   * **D. New Shiny-Object Pattern**: A new avoidance habit or distraction vector has crept in and needs to be added to Butterfly's radar.
2. **Clean Up & Re-Tune**:
   * Move stale or deprioritized commitments from Section 1 (`Active Commitments`) into Section 4 (`Chrysalis Parking Lot`) so the active plate is fresh, honest, and under the `WIP Limit`.
   * Update the North Stars, Mentor Archetype, or Coaching Intensity in `RBM_PROFILE.md`.
   * Append an entry to Section 5 (`Calibration Drift Log`) in `RBM_PROFILE.md` recording the date, why recalibration was triggered, and what changed.

---

## Step 3: Write `RBM_PROFILE.md` and `RBM_LEDGER.md`

Using the templates in `resources/templates/RBM_PROFILE.template.md` and `resources/templates/RBM_LEDGER.template.md`, write or update:
* `./RBM_PROFILE.md`
* `./RBM_LEDGER.md`

Confirm calibration is complete and share clickable links to both files.
