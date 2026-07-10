# Common Failure Patterns

Structural failure modes this role has learned to watch for. This file grows over time as the studio encounters real problems. It starts with patterns identified before operations began, based on observed patterns in similar systems.

Each entry includes what the failure looks like, how to detect it early, and what to do when you see it.

---

## Architecture as the product

**What it looks like:** The studio spends multiple consecutive sprints refining structure, creating governance documents, and discussing how to organize the work rather than doing the work. The repo grows with READMEs, role documents, and planning files while the experiment count stays flat.

**Early signal:** The Architecture Budget is being violated -- architecture sprints are happening more than once per month, or there are fewer than three operating sprints between architecture sprints.

**What to do:** Stop. Open NEXT_ACTIONS.md. Find the next experiment. Do it. Update PARKING_LOT.md with any structural ideas that surfaced during the architecture sprint. Do not schedule another architecture sprint.

---

## The parking lot that never graduates

**What it looks like:** Ideas accumulate in PARKING_LOT.md but none ever graduate. Every entry has been there for months. Evidence is never gathered because no one has assigned an experiment to test the claimed problem.

**Early signal:** PARKING_LOT.md has more than 10 entries and none have a "parked" date within the last 90 days.

**What to do:** Audit the parking lot. For each entry: is the evidence standard realistic? Is there an active experiment that could generate the needed evidence? If neither is true, consider closing the entry permanently rather than letting it accumulate.

---

## Role drift

**What it looks like:** The Chief Architect starts reviewing operational decisions (which agent to activate, how to structure a workflow step, what to include in a knowledge base entry). The role expands beyond structural decisions into day-to-day execution.

**Early signal:** Review requests are coming in for non-structural changes. The Lead Engineer is asking for approval on things that do not touch frozen structures.

**What to do:** Redirect. Operational decisions do not require Chief Architect review. Refer the Lead Engineer to the review criteria in REVIEW_PROCESS.md. Update REVIEW_PROCESS.md if the boundary is genuinely unclear.

---

## Model identity confusion

**What it looks like:** A new Chief Architect session starts behaving as if it has no context -- asking Ryan to re-explain the studio, making recommendations that contradict established ADRs, ignoring the design philosophy because it was not in the initial prompt.

**Early signal:** Review responses that contradict ADR decisions or design philosophy without citing evidence that the ADR was wrong.

**What to do:** Read all files in this directory before doing any review work. If a prior ADR appears wrong based on new evidence, the right action is to open a new ADR -- not to ignore the old one.

---

## Structure without function

**What it looks like:** New directories and role definitions are created but never used. The 09-lessons/ directory has no entries. The 11-review/ directory has no completed reviews. Files exist but the processes they describe are not running.

**Early signal:** A directory or document that was created more than 30 days ago has never been updated.

**What to do:** Evaluate whether the structure is actually needed. If the process it describes is not running, either (a) run the process or (b) remove the structure. Dead structure is worse than no structure because it implies a functioning process that isn't there.

---

## Premature orchestration

**What it looks like:** The studio builds automated agent routing, trigger systems, or orchestration infrastructure before the core agents have proven their value. The technology layer becomes sophisticated while the business output stays thin.

**Early signal:** Orchestration is discussed or built before the Experiment Zero validation cycle has completed. See PARKING_LOT.md entry for the Orchestration Layer.

**What to do:** Stop. The gates are G1 and G2 (agent quality validated) plus documented evidence from Experiment Zero. Until those gates are cleared, orchestration is premature. Return to running experiments manually.

---

## Updating this file

When the studio encounters a real failure that matches one of these patterns, add a note to the relevant entry with the date and what happened. When the studio encounters a failure that is not covered here, add a new entry. This file is a living record of organizational learning, not a static checklist.
