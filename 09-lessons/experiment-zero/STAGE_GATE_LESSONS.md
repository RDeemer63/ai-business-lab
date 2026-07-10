# Stage Gate Lessons — Experiment Zero

**Source:** Chief Architect Stage Gate review of PR #5
**Date:** 2026-07-09
**Applies to:** All future experiments

---

## Lesson 1: Never modify an experiment KPI to accommodate the current implementation.

Improve the implementation until it satisfies the original KPI, or record that the experiment failed.

**What happened:** The v2 validation plan estimated Ryan's time at 2h10m and quietly changed the acceptance threshold to "under 2h20m." The original Experiment Zero KPI is under 2 hours. The Chief Architect Stage Gate caught the shift and blocked the merge.

**What the team did:** Redesigned the email workflow instead of adjusting the KPI. Agents now prepare all 100 personalized email drafts before Day 0. Ryan spot-checks 5, approves the batch, and the send is triggered. Revised estimate: 1h45m.

**The rule:** The experiment defines the constraint. Change the organization. Do not change the experiment.

**Why this matters for every future experiment:** If KPIs shift to match estimates, they become meaningless. The studio's ability to learn depends on holding the standard fixed and measuring reality against it. A failed experiment that honestly records "we could not complete this under 2 hours" is more valuable than a passed experiment that moved the bar.

---

## Lesson 2: Stage gates work when they change decisions, not just document them.

**What happened:** PR #5 was ready to merge. The Chief Architect reviewed the actual files — not just the summary — and blocked on one remaining issue. The team did not argue for a variance. The team fixed the workflow.

**The rule:** A governance layer that can be argued around is not governance. When a stage gate says no, the answer is to satisfy the gate, not to negotiate with it.

---

## How these lessons propagate

The Knowledge Curator should incorporate Lesson 1 into the VALIDATE_BUSINESS_IDEA.md workflow template — add an explicit check: "Does this validation plan modify any KPI from the experiment definition? If yes, stop and redesign the implementation."

The Historian should reference this file in any future post-mortem where a KPI adjustment is proposed mid-experiment.
