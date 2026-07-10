# Decisions Not to Build

Things that look like good ideas but are not appropriate for the current phase, or that have been explicitly decided against. This file prevents re-litigating the same question every session.

Each entry explains what was proposed, why it was decided against, and what evidence would change the decision.

---

## Automated orchestration

**What it is:** An automated system that routes tasks between agents, triggers Claude Code on events, or runs multi-agent workflows without Ryan's involvement.

**Why not yet:** The core agents have not proven their value. Orchestrating unproven agents creates sophisticated failure modes. G1 and G2 gates must clear first. See PARKING_LOT.md.

**What changes this:** G1 and G2 cleared + Experiment Zero completed + documented evidence that manual routing is creating measurable bottlenecks.

---

## Intelligence Department formal structure

**What it is:** A named department with a department README, formal reporting structure, and defined roles for research and analysis functions.

**Why not yet:** In Phase 1, intelligence functions are handled by the Business Research agent and the Business Strategist. Creating a formal department adds coordination overhead without adding capability. The structure should emerge from proven workflow patterns.

**What changes this:** Three or more completed experiments where post-mortems identify coordination failure between intelligence functions.

---

## Studio Health Dashboard

**What it is:** A dashboard (file, app, or automated report) showing launch velocity, experiment completion rate, and agent utilization.

**Why not yet:** The studio has run zero experiments. There is nothing to measure. A dashboard built before data exists will measure the wrong things.

**What changes this:** Six weeks of operational data with at least three completed experiments.

---

## Weekly rhythm cadence (automated)

**What it is:** Automated prompts or calendar triggers that initiate weekly review sessions, architecture check-ins, or business pipeline reviews.

**Why not yet:** The studio's operational rhythm is not yet established. Automating a cadence before understanding the natural rhythm creates artificial overhead.

**What changes this:** Four consecutive operating weeks with documented sprint rhythm and a clear pattern of which reviews are actually valuable.

---

## Agent evaluation pipeline

**What it is:** A formal scoring and evaluation system for new agents from the library, with rubrics, comparison tables, and a standardized trial process.

**Why not yet:** AGENT_REGISTRY.md and SELECTION_GUIDE.md already handle agent evaluation adequately for Phase 1. A formal pipeline is overhead for the current volume.

**What changes this:** More than 10 agent evaluations in a single month, or documented evidence that the current evaluation process is producing wrong choices.

---

## Custom workflow engine

**What it is:** A code-based system that executes workflow steps, manages state between steps, and orchestrates agent handoffs programmatically.

**Why not yet:** Phase 1 workflows are documented as markdown files in `03-workflows/` and executed manually. A code-based engine adds engineering complexity without adding capability at the current volume.

**What changes this:** Demonstrated need in post-mortems: workflows that ran manually failed specifically because of coordination problems that a code engine would have prevented.

---

## Updating this file

When a new "not to build" decision is made, add it here with the same format. When a decision's conditions change and it moves from "not yet" to "now," remove the entry and create an ADR documenting the change. Do not delete entries silently -- move them with context.
