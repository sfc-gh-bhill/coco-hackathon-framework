---
project: "[YOUR PROJECT NAME]"
owner: "[YOUR NAME]"
use_case: "[ONE LINE DESCRIPTION — e.g., 'AI-powered claims triage using Cortex + Streamlit']"
start_time: "[HH:MM]"
target_demo_time: "[HH:MM]"
status: not_started
current_phase: 0
---

# Hackathon Plan — [YOUR PROJECT NAME]

> Copy this file, rename it to `PLAN_<your_project_name>.md`, fill in the bracketed fields, and work through it with CoCo phase by phase. At each gate, paste the gate line into chat and wait for CoCo to confirm before moving on.

---

## Phase 0 — Orient & Setup
**Time box:** ~15 minutes

Get grounded. The goal here is clarity, not code.

- [ ] Introduce yourself and your project to CoCo — tell it your name, use case, and what Snowflake features you want to use
- [ ] Ask CoCo to help you sharpen your project scope to 2–3 sentences max
- [ ] Confirm your target demo outcome: fill in → "At the end of the hackathon, I want to show **[WHAT THE JUDGE SEES AND HEARS]**"
- [ ] Decide on your project folder structure and ask CoCo to scaffold it
- [ ] Run: `cortex ctx remember "Project: [YOUR PROJECT NAME] — [ONE-LINE DESCRIPTION]"`

**Definition of Done:** I can clearly state what I'm building and what the demo looks like. ✓

> **Gate 0:** Paste this into CoCo when ready → `"Gate 0 complete. My project is [NAME]. I'm building [DESCRIPTION]. My demo outcome is [OUTCOME]. Ready for Phase 1."`

---

## Phase 1 — Requirements & Architecture
**Time box:** ~20 minutes

Decide what you're building before you build it. Scope creep kills hackathon projects.

- [ ] List your 3–5 core features needed for a working demo (not nice-to-haves — the minimum viable demo)
- [ ] Ask CoCo to sketch the architecture: data flow, major components, interfaces
- [ ] Identify your data source(s): real data, synthetic data, or Snowflake sample data (e.g., `SNOWFLAKE_SAMPLE_DATA`)
- [ ] Lock in your tech stack — fill in:
  - Frontend: `[Streamlit / no UI / other]`
  - Data layer: `[SQL / Snowpark / dbt / other]`
  - AI layer: `[Cortex LLM functions / Cortex Agents / Cortex Analyst / none]`
  - Storage: `[Snowflake tables / stages / other]`
- [ ] Save key decisions: `cortex ctx remember "[decision made and why]"`

**Definition of Done:** I have a 1-page architecture I could whiteboard for a judge. ✓

> **Gate 1:** Paste this into CoCo when ready → `"Gate 1 complete. Core features: [LIST]. Stack: [STACK]. Data source: [SOURCE]. Ready for Phase 2."`

---

## Phase 2 — Scaffold & Stub
**Time box:** ~30 minutes

Get something running, even if it's empty. A skeleton you can run beats a full design you can't.

- [ ] Create the project directory structure (ask CoCo to do this for you)
- [ ] Write stub files (`app.py`, `main.sql`, `queries.py`, etc.) with inline comments describing intent — no real logic yet
- [ ] Set up Snowflake connection and any required database objects (database, schema, tables, stages)
- [ ] Verify the app launches without errors — placeholder data, dummy UI, or just a `SELECT 1` is fine
- [ ] Checkpoint: save or commit your work so you have a known-good state to revert to

**Definition of Done:** The app launches without errors and I can see the skeleton of the UI or output. ✓

> **Gate 2:** Paste this into CoCo when ready → `"Gate 2 complete. Scaffold is running. No errors on launch. Ready for Phase 3."`

---

## Phase 3 — Core Build
**Time box:** ~90 minutes

This is the bulk of your build time. Stay focused — if a feature is taking too long, stub it and move on.

- [ ] **Feature 1:** `[FILL IN — e.g., 'Ingest CSV into Snowflake stage and load into table']`
- [ ] **Feature 2:** `[FILL IN — e.g., 'Run Cortex COMPLETE to summarize each record']`
- [ ] **Feature 3:** `[FILL IN — e.g., 'Display results in Streamlit with filter controls']`
- [ ] Connect real (or realistic synthetic) data to the UI — no more hardcoded test values
- [ ] Add basic error handling so the demo doesn't crash on bad or missing input
- [ ] End-to-end test: manually run the full demo flow from start to finish at least once

**Definition of Done:** A user can click through the full demo flow without hitting a crash. ✓

> **Gate 3:** Paste this into CoCo when ready → `"Gate 3 complete. All 3 core features working. Full flow tested. Ready for Phase 4."`

---

## Phase 4 — Polish & Demo Prep
**Time box:** ~30 minutes

A rough demo that you can narrate confidently beats a polished demo you fumble through.

- [ ] Fix the most visible rough edges — broken layout, leftover placeholder text, console errors
- [ ] Write a 2-minute demo script: what you click, what you say at each step
- [ ] Add at least one "wow moment" — an AI-generated insight, a chart that updates live, an unexpected finding in the data
- [ ] Prepare 3 talking points:
  1. The problem: `[FILL IN]`
  2. Your solution: `[FILL IN]`
  3. The Snowflake angle (what Snowflake feature makes this possible): `[FILL IN]`
- [ ] Do a full demo run-through out loud, end to end — time yourself

**Definition of Done:** I can demo this confidently in 3 minutes with no notes. ✓

> **Gate 4:** Paste this into CoCo when ready → `"Gate 4 complete. Demo script written. Wow moment in place. 3-minute run-through done. Ready for Phase 5 or final submission."`

---

## Phase 5 — Buffer / Stretch Goals
**Time box:** Remaining time

Only work on these if Phase 4 is fully done. Don't trade a polished demo for unfinished features.

- [ ] `[Stretch goal 1 — e.g., 'Add a second Cortex function for sentiment scoring']`
- [ ] `[Stretch goal 2 — e.g., 'Add a download button to export results as CSV']`
- [ ] `[Stretch goal 3 — e.g., 'Deploy to Streamlit in Snowflake']`

---

## Session Notes

### Key Decisions
> *Document the significant choices you made and why — useful for the Q&A after your demo.*

-
-
-

### Blockers Encountered
> *What slowed you down? What did you have to work around?*

-
-
-

### What I'd Do Next
> *If you had another 4 hours, what would you build or improve?*

-
-
-
