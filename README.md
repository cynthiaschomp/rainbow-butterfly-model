<p align="center">
  <img src="docs/assets/readme-header.svg" width="560" height="122" alt="Rainbow Butterfly Model">
</p>

<p align="center"><strong>Strategize with a Rainbow. Execute with a Butterfly.</strong></p>

<p align="center">
  <a href="#install">Install</a> &ensp;·&ensp;
  <a href="#calibrate-first">Calibrate First</a> &ensp;·&ensp;
  <a href="#the-agents">The Agents</a> &ensp;·&ensp;
  <a href="#skills--commands">Skills & Commands</a> &ensp;·&ensp;
  <a href="#recalibrating-when-things-feel-off">Recalibration</a>
</p>

<br>

The **Rainbow Butterfly Model (`rbm`)** is an open-source business mentorship and executive coaching plugin for AI coding agents (Antigravity, Claude Code, Codex).

While the **Elephant-Goldfish Model (`egm`)** stress-tests *what* you are building from a technical and user-critic perspective, the **Rainbow Butterfly Model (`rbm`)** governs *why, when, and how profitably* you run your business:

* 🌈 **Rainbow (`rbm-rainbow`) — The Business Mentor:** Evaluates every idea, offer, price point, and roadmap choice across the **7-Wavelength Commercial Spectrum** (Market/Buyer Urgency, Unit Economics, Portfolio Alignment, Asset Leverage, Opportunity Cost, Commercial Risk/Moat, and 6–36 Month Scale Path).
* 🦋 **Butterfly (`rbm-butterfly`) — The Business Coach:** Protects your focus, catches "productive procrastination" (hiding in code to avoid sales, shipping, or follow-ups), enforces your active Work-In-Progress (`WIP`) limit, and drives your **One Wing Flap**—the single highest-leverage business action for today.

---

## Install

### Antigravity CLI (`agy`)

```sh
agy plugin install https://github.com/cynthiaschomp/rainbow-butterfly-model
```

Or clone directly into your global Antigravity plugins directory:

```sh
git clone https://github.com/cynthiaschomp/rainbow-butterfly-model ~/.gemini/config/plugins/rbm
```

### Claude Code / Codex

Clone or add the repository to your agent's plugin directory and start a new session so the subagents (`rbm-rainbow`, `rbm-butterfly`, `rbm-synthesizer`) and skills (`rbm-calibrate`, `rbm-council`, `rbm-mentor`, `rbm-coach`) are discovered.

---

## Calibrate First

Every founder, agency, and product studio operates differently. **Before using Rainbow or Butterfly, run `/rbm-calibrate`.**

```text
/rbm-calibrate
```

The calibration workflow interviews you across 5 dimensions and generates two living ground-truth files in your workspace:

1. **`RBM_PROFILE.md` (Your Calibration Profile):**
   * Your business pillars/umbrellas and revenue engines
   * Verified financial baseline & floor price *(RBM never hallucinates or guesses financial figures)*
   * Current 90-day Strategic North Stars and explicit **Anti-Goals**
   * **Rainbow Mentor Voice:** `Board-Level Commercial Strategist`, `Bootstrapped Unit-Economics Operator`, or `Product-Led Growth Architect`
   * **Butterfly Coach Intensity:** `Gentle Compass`, `Firm Momentum Partner`, or `Ruthless Gatekeeper (Finish Your Plate First)`
   * Your personal **"Productive Procrastination" / Shiny-Object triggers**
2. **`RBM_LEDGER.md` (Your Execution & Decision Ledger):**
   * **Section 1:** Active Commitments ("On The Plate") + your max `WIP Limit`
   * **Section 2:** Today's **One Wing Flap** & Definition of Done
   * **Section 3:** **Rainbow Decision Log** (Why you said `GO`, `PARKED`, or `NO`)
   * **Section 4:** **The Chrysalis Parking Lot** (Where good ideas wait until your active commitments ship)
   * **Section 5:** **Completed Flights** (Shipped wins)

---

## The Agents

| Agent | Persona | Core Responsibility |
| :--- | :--- | :--- |
| **`rbm-rainbow`** | 🌈 **Business Mentor** | Evaluates commercial logic, pricing, margins, positioning, and asset leverage across the 7 Commercial Wavelengths. Issues a clear `GO`, `CONDITIONAL / SCOPE-DOWN`, `CHRYSALIS PARK`, or `NO` verdict. |
| **`rbm-butterfly`** | 🦋 **Business Coach** | Audits your active commitments in `RBM_LEDGER.md`, intercepts shiny-object detours, enforces your WIP limit, asks the sharp coaching question, and defines your **One Wing Flap**. |
| **`rbm-synthesizer`** | 🌈 + 🦋 **Council Coordinator** | Runs Rainbow and Butterfly in tandem when you say *"Rainbow Butterfly it!"* so strategy and execution stay locked together. |

---

## Skills & Commands

| Skill | Trigger / Command | Use it when… |
| :--- | :--- | :--- |
| <img src="skills/rbm-calibrate/assets/icon.svg" width="18" height="18" align="top" alt=""> **[`rbm-calibrate`](skills/rbm-calibrate/SKILL.md)** | `/rbm-calibrate` or *"Calibrate Rainbow Butterfly"* | First-time setup, or anytime your goals shift or coaching/mentorship feels off. |
| <img src="skills/rbm-council/assets/icon.svg" width="18" height="18" align="top" alt=""> **[`rbm-council`](skills/rbm-council/SKILL.md)** | `/rbm-council` or *"Rainbow Butterfly it!"* | You want **both** Rainbow's 7-wavelength business critique and Butterfly's accountability & action plan. |
| <img src="skills/rbm-mentor/assets/icon.svg" width="18" height="18" align="top" alt=""> **[`rbm-mentor`](skills/rbm-mentor/SKILL.md)** | `/rbm-mentor` or *"Call Rainbow"* | You need business expert eyes on pricing, an offer, a client deal, or product strategy. |
| <img src="skills/rbm-coach/assets/icon.svg" width="18" height="18" align="top" alt=""> **[`rbm-coach`](skills/rbm-coach/SKILL.md)** | `/rbm-coach` or *"Call Butterfly"* | Morning focus check-in, weekly review, or when you feel pulled in 10 directions. |

---

## Recalibrating When Things Feel Off

Businesses evolve through seasons. If Rainbow feels too rigid (or too permissive), if Butterfly is pushing on stale goals, or if your `RBM_LEDGER.md` plate has accumulated clutter, simply run:

```text
/rbm-calibrate Things feel off — let's recalibrate.
```

**Recalibration Mode** diagnoses 4 types of drift:
1. **Strategic Drift:** Updates your 90-day North Stars and Anti-Goals.
2. **Tone / Pushback Mismatch:** Adjusts Rainbow's strictness (1–5) or Butterfly's intensity (`Gentle Compass` ↔ `Firm Momentum Partner` ↔ `Ruthless Gatekeeper`).
3. **Plate Overload (Ledger Bankruptcy):** Moves stale commitments into the **Chrysalis Parking Lot** so your active plate is clean and under your `WIP Limit`.
4. **New Shiny-Object Pattern:** Adds newly discovered procrastination triggers to Butterfly's radar and logs the change in your `Calibration Drift Log`.

---

## License

[Apache 2.0](LICENSE)
