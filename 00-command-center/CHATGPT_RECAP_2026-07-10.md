# ChatGPT Recap — 2026-07-10

**From:** Lead Engineer + Ryan
**To:** Chief Architect
**Re:** Session recap — constitutional rule, Experiment 001 Gate 1, GHL findings, parking lot additions

---

## What Happened This Session

Three things were accomplished. Here they are in order.

---

### 1. Constitutional Rule + Governance Cleanup

Before Gate 1 started, we implemented the constitutional rule you proposed last session.

**OPERATING_PRINCIPLES.md updated to v1.1.** A preamble now sits above Principle 1:

> "No operating principle may be added unless it can be traced to a specific experiment, decision, or post-mortem. The source must be cited in the principle itself."

The rule is itself sourced from the evidence of Principle 12 — the first principle this organization earned rather than invented.

**PRINCIPLE_REGISTRY.md parked.** Added to PARKING_LOT.md. Evidence needed before it graduates: 10+ principles and 2+ instances where knowing a principle's lineage changed a decision.

All changes merged to main via PR #12.

---

### 2. Experiment 001 Gate 1 — PASS

Ryan approved the experiment. Gate 1 was built and passed the same session.

**What was built:**

A live GHL demo in a dedicated sandbox sub-account ("AI Business Lab — Demo Account") created via the GHL API. The sub-account contains:

- Lead Recovery Pipeline (6 stages: New Lead → Contacted → Qualified → Booked → Won → Lost)
- Contractor Consultation calendar
- A complete 7-message SMS qualification conversation — simulated HVAC homeowner lead "Mike Thompson" texts in, the AI acknowledges immediately, qualifies service type and urgency, confirms geographic coverage, gets buy-in, drops a booking link
- Pipeline opportunity at the "Booked" stage

Ryan's credibility review: "This is pretty good." **Gate 1: PASS.** Confidence score: 60% → 75%.

**What to show contractors in Gate 2:** Ryan screen-shares the GHL conversation thread. The lead's experience is fully built out. No live AI needed for Gate 2 — the conversation is pre-built and demonstrates the promise clearly.

---

### 3. GHL AI API Investigation — Key Finding

During the build, we investigated whether GHL's Conversations AI (their "AI Employee" feature) is configurable via API.

**Finding: no.** GHL's Conversations AI configuration is UI-only. No public API endpoints exist for bot creation, personality configuration, or training. The public API exposes contacts, conversations, pipelines, calendars — but not AI feature setup.

**A2P flagged.** SMS at scale requires A2P 10DLC registration (~$15/month, 2-4 week approval). Does not block Gate 2 screen-share demos. Becomes real at Gate 3+ when a paying client's leads start texting in. Action: Ryan starts registration in parallel with Gate 2.

---

### 4. New Parking Lot Addition — Claude-Powered GHL Webhook Layer

During the API investigation, we found a better path than GHL's native AI:

**The architecture:**
```
Lead texts in → GHL receives SMS → GHL Workflow fires (built once in UI)
→ Webhook hits our server → Claude API generates response with contractor context
→ Server posts reply via GHL conversations API → Lead gets AI reply
```

**Why it's better than GHL native:**
- Claude outperforms GHL's LLM
- Prompts fully customizable per contractor (trade, service area, urgency rules, booking logic)
- New clients = new prompt, not new UI build
- We own the intelligence layer

**Why it's parked:** Scope creep for Gate 1. Gate 2 is a screen-share demo. The webhook server becomes relevant when Gate 3 passes and setup speed matters for a paying client.

**Build estimate when ready:** ~100-line Node.js server, free deploy on Railway/Render, one GHL UI workflow built once. Ryan has Vercel available.

This is the first concrete capability that belongs in the Capability Library you proposed. It's parked — not discarded.

---

## Current Experiment Status

| Gate | Question | Status | Confidence |
|------|----------|--------|------------|
| Gate 1 | Can we demonstrate the promise? | PASS | 75% |
| Gate 2 | Do contractors want it? | NOT STARTED | — |
| Gate 3 | Will they pay? | NOT STARTED | — |

**Gate 2 requires Ryan:** 3 contractor demos, screen-share the GHL conversation, ask both required questions. No engineering needed until Gate 2 results come back.

---

## What's in the Repo

All of this is on main:

- `04-experiments/experiment-001/DEMO_BUILD.md` — full build doc, credentials reference, Wizard-of-Oz notes, production setup path
- `04-experiments/experiment-001/GATE_1_RESULT.md` — Gate 1 outcome, A2P constraint, Gate 2 authorization
- `04-experiments/experiment-001/RYAN_TIME_LOG.md` — time tracking template
- `00-command-center/OPERATING_PRINCIPLES.md` — v1.1 with constitutional rule
- `00-command-center/PARKING_LOT.md` — Claude webhook layer added

---

## Questions for Chief Architect

1. **Gate 2 prep:** Ryan will screen-share the pre-built conversation. Should we give him a one-page script for how to frame the demo to a contractor — what to say before he pulls up the screen, how to introduce the product, how to ask the two required questions naturally? Or is that over-engineering Gate 2?

2. **The factory model:** Your Phase 2 framing (factories, not agents) is exactly right. The Claude webhook architecture is the first concrete "capability" for the Capability Library. When Gate 3 passes, should the first build session focus on that capability — or is there a sequencing argument for something else first?

3. **A2P timing:** Registering the brand now means it's approved by the time Gate 3 needs it. Any reason NOT to start registration immediately, even before Gate 2 results are in?
