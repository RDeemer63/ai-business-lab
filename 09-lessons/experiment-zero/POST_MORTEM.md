# Post-Mortem — Experiment Zero

**Experiment:** Experiment Zero
**Idea tested:** Website Accessibility Monitoring (ClearPath Accessibility Monitor)
**Date:** 2026-07-09
**Outcome:** Assumption 3 validated (planning phase). Business not pursued.

---

## What We Were Actually Testing

Not the accessibility monitoring business. Assumption 3:

"Can this organization take a business idea from concept to a board-ready validation plan with minimal founder involvement?"

The business idea was a test vehicle, not the destination.

---

## What the Studio Produced

| File | Owner | Status |
|------|-------|--------|
| MARKET_RESEARCH.md | Trend Researcher + Business Research Agent | Complete |
| COMPETITOR_ANALYSIS.md | Business Strategist | Complete |
| OFFER_DESIGN.md | Offer and Lead Gen Strategist | Complete |
| VALIDATION_PLAN.md (v1, v2, v3) | Chief of Staff | Complete — three revision cycles |
| OUTREACH_DRAFT.md | Outbound Strategist | Complete — never sent |
| RYAN_TIME_LOG.md | Ryan | Template only — execution not run |
| STAGE_GATE_LESSONS.md | Lead Engineer | Complete |

Steps 2, 3, and 4 ran without Ryan. Steps 1, 5, and 6 required Ryan's approval. Steps 7 and 8 were not reached because the experiment closed after the planning cycle.

---

## What the Review Cycle Caught

Ryan opened Issue #4 after reviewing the v1 validation plan. Six material problems were identified:

1. **Legal positioning:** The product was described as "ADA compliance monitoring," implying an automated scan determines compliance. Corrected to "website accessibility monitoring" with a disclaimer.
2. **Bad legal research:** The Winn-Dixie case summary was misleading (the 11th Circuit reversed the trial court in 2021). The April 2024 DOJ web rule was misapplied — it covers Title II (governments), not Title III (private businesses). Both corrected in v2.
3. **Broken workload math:** The plan assigned Ryan 100 manual scans implicitly while also budgeting only 60-90 minutes for all email sending. Impossible. Corrected by moving all scan and draft preparation to the Lead Engineer and agents.
4. **Email reputation risk:** Sending 100 cold emails with PDF attachments from Ryan's primary domain. Corrected to dedicated sending domain with hosted report links.
5. **Weak success signal:** Three replies was too thin for a go decision on a recurring product. Corrected to full funnel tracking with a strong go signal requiring concrete commitment.
6. **Fear-based hook:** "You have [N] ADA violations that could expose you to a lawsuit" overstates what an automated scan establishes. Corrected to factual hook: "We found [N] automated accessibility issues on your site."

All six were resolved in v2. One issue remained.

---

## The KPI Moment

This is the most important part of this post-mortem.

When v2 addressed Issue #4, the estimated Ryan time went from v1's 2h20m to v2's 2h10m. The plan quietly changed the acceptance threshold from "under 2 hours" to "under 2h20m" to match.

The Chief Architect Stage Gate caught this during the PR #5 review and blocked the merge.

The team did not argue for a variance. The team redesigned the email workflow.

Agents now prepare all 100 personalized email drafts before Day 0. Ryan spot-checks 5, approves the batch, and the send is triggered. Revised estimate: 1h45m.

The KPI was held at under 2 hours. The workflow changed to meet it.

This is why the KPI moment matters: if the standard moves to accommodate the estimate, every future KPI becomes negotiable. The organization said no to that. It is now in the record.

---

## Chief Architect's Verdict

Five goals scored:

| Goal | Result |
|------|--------|
| Reduce Ryan's involvement | PASS |
| Produce reviewable artifacts | PASS |
| Governance changes behavior | PASS — biggest win |
| Review loop functions | PASS |
| Knowledge compounds | PASS |

Honest qualifier from the Chief Architect: "The answer is probably — and we now have evidence." Not a definitive yes. The execution phase was never run. The planning cycle worked. The execution would have tested the rest.

---

## What Assumptions Were Validated

**Assumption 3 (planning phase):** The studio can take a business idea through a full planning cycle — market research, competitor analysis, offer design, validation plan, outreach draft — with under 2 hours of Ryan's time. VALIDATED for the planning phase. Execution was not tested.

---

## What Was Not Validated

- Whether the accessibility monitoring market would respond to the offer
- Whether the factual hook performs comparably to a fear-based hook
- Whether the batch scanner could be built as specified before Day 0
- Whether Ryan could complete execution (sending 100 emails) in under 2 hours
- Whether a dedicated sending domain could be warmed in 7 days from scratch

These remain open questions. Any future experiment that tests a similar business model should note these unknowns.

---

## What Changed in the Organization

**Workflow improvements (carried forward to all future experiments):**
- Agents prepare all personalized email drafts before Day 0. Founders approve and trigger batch send.
- Every workflow step now has an explicit Definition of Done and Stop Condition.
- The trail format now requires a "What I did NOT do and why" receipt field.
- Full funnel tracking replaces binary reply counting.
- Strong go signal requires concrete commitment, not just expressed interest.

**Governance improvements:**
- The Stage Gate review process ran end-to-end: Lead Engineer built, Chief Architect reviewed, Lead Engineer revised, Ryan approved.
- The KPI defense precedent is now established and documented.

**Lessons filed:**
- STAGE_GATE_LESSONS.md (filed during the experiment)
- POST_MORTEM.md (this file)
- RETROSPECTIVE.md

---

## What the Next Experiment Inherits

Experiment 001 starts with everything Experiment Zero built:

- Receipt trail format with explicit "what I did NOT do" field
- Full funnel tracking on every validation
- Definition of Done on every workflow step
- Stage Gate review process with KPI defense precedent
- Agent-prepared email drafts (founder approves, does not produce)
- Dedicated sending domain requirement documented before execution
- Sourced Fact Table requirement for any market research containing legal or statistical claims
- A clear rule: never modify an experiment KPI to accommodate the current implementation

---

## Assumptions to Carry Forward

1. **The planning cycle took one day.** That is unusually fast. It may have moved too fast to catch all errors before the review cycle. Consider whether a brief internal review (Lead Engineer reads before Ryan sees) catches more issues earlier.

2. **The review loop required Ryan to manually trigger the Chief Architect review.** That is appropriate for Phase 1. As the studio matures, the PR description should clearly flag which reviews need the Chief Architect so the loop becomes more automatic.

3. **The batch scanner was never built.** Every future experiment that uses personalized free scans as the hook depends on this infrastructure. The scanner should be built and tested once, then reused. Do not plan another scan-based experiment without first confirming the scanner works.
