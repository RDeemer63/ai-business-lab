# Experiment 001 — AI-Driven Contractor Lead Recovery

**Status:** IN PROGRESS — Gate 1 (Ryan approved 2026-07-10)
**Type:** Business validation (three gates)
**Date defined:** 2026-07-10
**Experiment identifier:** 001

---

## Revision Log

| Version | Date | Changes |
|---------|------|---------|
| v1 | 2026-07-10 | Initial definition |
| v2 | 2026-07-10 | Investment Committee approval conditions applied: hypothesis tightened, Gate 1 renamed, required interview question added, price testing added to Gate 3, 2.5-hour budget exception documented, Confidence Score added per gate |

---

## The Hypothesis

Will contractors pay recurring revenue to recover leads they are currently losing through automated follow-up?

The AI is the delivery mechanism. Contractors do not buy AI. They buy more jobs. This hypothesis is implementation-agnostic — GHL is the current tool, but the experiment does not require it. If Tulboxx becomes the better platform mid-experiment, the hypothesis stays. The implementation changes.

---

## Why This Experiment

AI Lead Follow-Up scored highest in the pipeline under the full six-metric framework:

| Metric | Score | Rationale |
|--------|-------|-----------|
| Business quality | 4.0 | Real pain, recurring revenue, AI-deliverable |
| Ryan fit | 4.0 | Existing GHL expertise, contractor relationships, Tulboxx |
| Job risk | 3.0 | Moderate — client relationships required, but delivery is automated |
| Strategic leverage | 5.0 | Platform capability applicable across Tulboxx, Throttled Up, future ventures |
| Reusable capability | 5.0 | Workflow reusable for estimates, invoices, reviews, maintenance reminders |
| Portfolio synergy | 5.0 | Direct Tulboxx roadmap input; strengthens Throttled Up marketing clients |
| Knowledge yield | 5.0 | Failure teaches: contractor willingness to automate sales, CRM expectations, pricing, objections, Tulboxx feature priority |

**The bigger picture:** Lead follow-up is the narrowest beachhead for an AI customer lifecycle engine. The same capability eventually handles estimate follow-ups, unpaid invoice reminders, review requests, maintenance reminders, and warranty check-ins. Today it recovers lost leads. The experiment tests the beachhead only.

---

## Founder Time Budget

**Total estimated Ryan time: under 2.5 hours**

This intentionally exceeds the Experiment Zero founder-time KPI of under 2 hours. The reason is documented:

Experiment Zero validated a planning cycle — research, analysis, offer design, outreach drafts. Ryan's role was review and approval. Experiment 001 is the first venture requiring live customer discovery. Ryan must run the demos and the pricing conversations personally. No agent can substitute for that in Gate 2 or Gate 3.

Future experiments requiring live customer discovery should seek to reduce this back toward 2 hours by tightening demo scripts, pre-qualifying contractors before booking the call, and reducing the number of demos needed for a signal.

If the founder time budget drifts upward again without a documented reason, flag it.

---

## Three Gates

This experiment runs as three sequential gates. Each gate answers exactly one question. A gate can fail without killing the entire venture — it identifies precisely where the problem lives.

**Rule:** Each gate answers ONE question. Not two. Not three.

---

### Gate 1 — Can we demonstrate the promise?

**One question:** Can we make contractors believe this works before we fully build it?

**Confidence before Gate 1:** 60% (we believe this is buildable, but haven't proven the demo is credible to a real contractor)

**What this gate is not:** A software engineering milestone. Gate 1 passes when the promise is demonstrated credibly — not when the engineering is complete. Acceptable delivery methods include a working GHL flow, a Wizard-of-Oz flow with a manual backend, or a high-fidelity mockup walkthrough. The goal is credibility, not code.

**Definition of Done:** Ryan has walked through the demo as if he were a lead contacting an HVAC or plumbing contractor. The interaction qualifies the lead and either books or escalates naturally. Ryan would show it to a real contractor client without embarrassment.

**Success:** Demo passes Ryan's credibility test. Gate 2 begins.

**Failure:** Demo requires too much manual setup per client to be scalable, or the conversation quality would embarrass Ryan in front of a client.

**Stop condition:** If the demo build reveals that the tools cannot produce a credible conversation without significant custom development beyond the experiment's scope, flag before Gate 2. Do not run Gate 2 against a failing demo.

**Owner:** Lead Engineer
**Ryan required:** Yes — final credibility review before Gate 2
**Ryan time:** 30 minutes

**Confidence after Gate 1:** 75%
**Why it changed:** Demo built and passed Ryan's credibility test. GHL API investigation revealed native Conversations AI is UI-only — but this invalidated a technical assumption, not the hypothesis. Claude webhook architecture identified as a better implementation path. Confidence gap (25%) = uncertainty about whether contractors will respond to the demo the way Ryan did.
**Evidence:** `04-experiments/experiment-001/GATE_1_RESULT.md`

---

### Gate 2 — Do contractors want it?

**One question:** Will contractors who see this demo ask how to get it?

**Confidence before Gate 2:** _____%

**Test method:** Walk 3 contractors through the live demo. No price mentioned during the demo. End each session with two questions:

1. "Would this be useful for your business?"
2. **Required:** "If you didn't buy this, what would be missing?"

The second question is not optional. It surfaces trust problems, pricing objections, feature gaps, and positioning problems. Record the contractor's answer verbatim — it becomes product requirements regardless of whether the gate passes.

**Definition of Done:** Three demos conducted. Both questions answered by each contractor. Each response classified as: Strong Interest / Mild Interest / No Interest. Verbatim answers to "what would be missing" recorded.

**Success:** 2 of 3 express strong interest or ask how to get it.

**Failure:** 0 of 3 express genuine interest.

**Inconclusive:** 1 of 3 expresses interest — run 2 more demos before calling it.

**Stop condition:** If the first contractor's response reveals a fundamental misunderstanding of the product, pause and refine the demo or positioning before continuing. Do not run all three demos against a broken framing.

**Owner:** Ryan (demos), Chief of Staff (results documentation)
**Ryan required:** Yes — Ryan runs all demos
**Ryan time:** 60-90 minutes (3 demos at 20-30 minutes each)

**Confidence after Gate 2 (fill in):** _____%

---

### Gate 3 — Will they pay?

**One question:** Will a contractor with genuine interest commit to a recurring payment before the system is fully built?

**Confidence before Gate 3:** _____%

**Test method:** Present pricing to Gate 2 strong-interest contractors. Test three price points — one per contractor — to gather qualitative pricing reactions:

| Contractor | Price point | Their words (record verbatim) |
|------------|------------|-------------------------------|
| Contractor A | $197/month | |
| Contractor B | $297/month | |
| Contractor C | $397/month | |

Listen for specific language: "That's cheap," "That's reasonable," "That's expensive." These words are evidence. Three conversations are not statistically significant — but the qualitative reactions map the pricing landscape before the full build.

Anchor every price with: "Most contractors recover that cost with one additional job per month."

**Definition of Done:** Pricing presented to all Gate 2 strong-interest contractors. Commitment status and verbatim pricing reactions recorded for each.

**Success:** At least 1 contractor commits — verbal agreement, written confirmation, or deposit.

**Failure:** No commitments after pricing is presented across all three price points.

**Inconclusive:** Strong interest but consistent objection to the price regardless of point — warrants a pricing iteration before declaring failure.

**Stop condition:** If every contractor expresses genuine interest but won't commit without seeing a live client system first, that is a signal about the sales motion, not the product. Document it and escalate to Ryan. Do not build to overcome this without explicit authorization.

**Owner:** Ryan (pricing conversations), Chief of Staff (documentation)
**Ryan required:** Yes — Ryan conducts all pricing conversations
**Ryan time:** 30-45 minutes

**Confidence after Gate 3 (fill in):** _____%

---

## The Tulboxx Question

This question is not answered during the experiment. It is the first decision *after* Gate 3 passes.

If Gate 2 and Gate 3 both pass, Ryan and the Investment Committee ask: does this belong inside Tulboxx or as a standalone product? Tulboxx already has contacts, estimates, pipeline, jobs, and invoices. Lead follow-up naturally lives there. If contractors pay for it separately first, that is market research for a Tulboxx feature — not necessarily a standalone company.

**The permanent rule this experiment is documenting:** Do not answer tomorrow's portfolio question with today's experiment. Validate the value. Then decide where it lives.

---

## What Failure Teaches

Even if all three gates fail, this experiment produces reusable knowledge:

- Contractor willingness to automate their sales process
- Which objections appear and how they phrase them
- CRM and GHL expectations in the contractor market
- Pricing sensitivity across the $197-$397 range
- Which Tulboxx features contractors actually want
- Whether the Throttled Up client base is a better initial audience than cold outreach

Knowledge yield: 5/5. Failure is as valuable as success.

---

## Experiment Scorecard (fill in after completion)

| Metric | Target | Actual |
|--------|--------|--------|
| Gate 1 pass | Demo passes Ryan credibility test | |
| Gate 2 pass | 2 of 3 strong interest | |
| Gate 3 pass | 1 commitment | |
| Gate 3 pricing reactions | Verbatim recorded for all 3 price points | |
| "What would be missing" answers | Recorded verbatim for all 3 contractors | |
| Ryan total time | Under 2.5 hours | |
| Contractors demoed | 3 minimum | |
| Knowledge base entries | At least 2 | |
| Tulboxx roadmap inputs | At least 1 | |

---

## Output Files

All go in `04-experiments/experiment-001/`:

| File | Owner | Content |
|------|-------|---------|
| DEMO_BUILD.md | Lead Engineer | What was built, delivery method chosen, known limitations |
| GATE_1_RESULT.md | Lead Engineer + Ryan | Demo credibility review outcome, confidence score |
| GATE_2_LOG.md | Ryan | Contractor reactions, verbatim "what would be missing" answers, confidence score |
| GATE_3_LOG.md | Ryan | Pricing reactions verbatim, commitment status, confidence score |
| RESULT.md | Chief of Staff | Final outcome across all three gates, go/no-go, Tulboxx recommendation |
| RYAN_TIME_LOG.md | Ryan | Time per touchpoint |

Post-experiment:
- `09-lessons/experiment-001/POST_MORTEM.md`

---

## Ryan Approval

This experiment definition is not active until Ryan approves it.

**Ryan Approval:**

Name: ____________________________
Date: ____________________________
Approved as written / Approved with the following changes:

_________________________________________________________

---

## To Start This Experiment

Ryan approves this document. Lead Engineer begins Gate 1 (demo build). Ryan's first touchpoint is the Gate 1 credibility review.
