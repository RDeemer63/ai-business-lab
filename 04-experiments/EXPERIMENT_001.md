# Experiment 001 — AI-Driven Contractor Lead Recovery

**Status:** DEFINED — pending Ryan approval
**Type:** Business validation (three gates)
**Date defined:** 2026-07-10
**Experiment identifier:** 001

---

## The Hypothesis

Can we recover revenue for contractors using AI-driven follow-up — and will they pay a recurring monthly fee for it?

This is implementation-agnostic. GHL is the current tool of choice. If Tulboxx becomes the better platform mid-experiment, the hypothesis does not change. Only the implementation does.

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
| **Knowledge yield** | **5.0** | Failure teaches: contractor willingness to automate sales, CRM expectations, pricing, objections, Tulboxx feature priority |

**The bigger picture:** Lead follow-up is the narrowest beachhead for an AI customer lifecycle engine. If the experiment succeeds, the same capability handles estimate follow-ups, unpaid invoice reminders, review requests, maintenance reminders, and warranty check-ins. Today it recovers lost leads. Eventually it manages the entire contractor customer relationship.

---

## Three Gates

This experiment runs as three sequential gates. Each gate has a pass/fail definition. A gate can fail without killing the entire venture — it identifies where the problem lives.

### Gate 1 — Can we build a believable demo?

**Hypothesis:** We can build a working GHL AI conversation flow for a contractor lead scenario that a real contractor would find credible.

**Definition of Done:** A working demo exists. Ryan has walked through it as if he were a lead contacting an HVAC or plumbing contractor. The AI responds naturally, qualifies the lead, and books or escalates appropriately.

**Success:** Demo runs cleanly. Ryan would show it to a contractor client without embarrassment.

**Failure:** Demo requires too much manual setup per client to be scalable, or the AI conversation quality is not credible.

**Stop condition:** If the demo build reveals that GHL's AI capabilities cannot produce a credible conversation without significant custom development, flag before Gate 2. Do not run Gate 2 against a demo that does not pass Gate 1.

**Owner:** Lead Engineer
**Ryan required:** Yes — final review of the demo before Gate 2 begins
**Ryan time:** 30 minutes

---

### Gate 2 — Will contractors ask for it?

**Hypothesis:** When contractors see a working demo of AI lead recovery, at least 1 in 3 will ask how to get it.

**Test method:** Walk 3 contractors through the live demo. No price mentioned. End with: "This is something we're testing — would this be useful for your business?" Count: how many ask "how do I get this?" or equivalent.

**Definition of Done:** Three demos conducted. Results logged. Each contractor's response classified as: Strong Interest / Mild Interest / No Interest.

**Success:** 2 of 3 express strong interest or ask to move forward.

**Failure:** 0 of 3 express genuine interest.

**Inconclusive:** 1 of 3 expresses interest — run 2 more demos before calling it.

**Stop condition:** If the first contractor's response reveals a fundamental misunderstanding of the product (they think we're building something we're not), pause and refine the demo before continuing.

**Owner:** Ryan (demos), Chief of Staff (results documentation)
**Ryan required:** Yes — Ryan runs the demos
**Ryan time:** 60-90 minutes (3 demos at 20-30 minutes each)

---

### Gate 3 — Will they pay recurring money?

**Hypothesis:** Contractors who expressed strong interest in Gate 2 will commit to a recurring monthly payment before the full system is built.

**Test method:** Present pricing to Gate 2 strong-interest contractors. Ask for a commitment — verbal, written, or a deposit. Do not build the full system before receiving a commitment signal.

**Price to test:** $297/month (from original research). Anchored as: "Less than one recovered job per month pays for itself."

**Definition of Done:** Pricing presented to all strong-interest contractors. Commitment status logged for each.

**Success:** At least 1 contractor commits (verbal agreement, written confirmation, or deposit).

**Failure:** No commitments after pricing is presented.

**Inconclusive:** Strong interest but consistent objection to the price point — warrants a pricing iteration.

**Stop condition:** If every contractor expresses interest but won't commit without seeing a "live" client system first, that is a signal about the sales process, not the product. Document and escalate to Ryan before building.

**Owner:** Ryan (pricing conversation), Chief of Staff (documentation)
**Ryan required:** Yes — Ryan conducts the pricing conversation
**Ryan time:** 30-45 minutes

---

## The Tulboxx Question

If Gate 2 and Gate 3 both pass, the first decision is not "build the standalone business." It is:

**Does this belong inside Tulboxx?**

Tulboxx already has contacts, estimates, pipeline, jobs, and invoices. Lead follow-up naturally belongs there. If contractors pay for it separately first, that is market research for a Tulboxx feature — not necessarily a standalone company.

The decision between standalone product and Tulboxx feature is a Ryan and investment committee decision. It happens after Gate 3 passes, not before.

---

## What Failure Teaches

Even if all three gates fail, this experiment produces reusable knowledge:

- Contractor willingness to automate their sales process
- Which objections appear and how they phrase them
- CRM and GHL expectations in the contractor market
- Pricing sensitivity at the $297/month level
- Which Tulboxx features are worth prioritizing
- Whether the Throttled Up client base is a better initial audience than cold outreach

Knowledge yield: 5/5. Failure is as valuable as success.

---

## Experiment Scorecard (fill in after completion)

| Metric | Target | Actual |
|--------|--------|--------|
| Gate 1 pass | Demo runs cleanly | |
| Gate 2 pass | 2 of 3 strong interest | |
| Gate 3 pass | 1 commitment | |
| Ryan total time | Under 2.5 hours | |
| Contractors demoed | 3 minimum | |
| Knowledge base entries | At least 2 | |
| Tulboxx roadmap inputs | At least 1 | |

---

## Output Files

All go in `04-experiments/experiment-001/`:

| File | Owner | Content |
|------|-------|---------|
| DEMO_BUILD.md | Lead Engineer | What was built, how it works, known limitations |
| GATE_1_RESULT.md | Lead Engineer + Ryan | Demo review outcome |
| GATE_2_LOG.md | Ryan | Contractor demo results, verbatim reactions where possible |
| GATE_3_LOG.md | Ryan | Pricing conversation outcomes, commitments or objections |
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

Ryan approves this document. Lead Engineer begins Gate 1 (demo build). Ryan's first touchpoint is the Gate 1 demo review.
