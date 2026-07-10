# Experiment 001 — Gate 1 Demo Build

**Status:** IN PROGRESS
**Owner:** Lead Engineer
**Started:** 2026-07-10
**Goal:** A GHL AI conversation flow Ryan can walk through as a lead contacting a contractor. The AI qualifies the lead and books or escalates naturally. Ryan would show it to a real contractor client without embarrassment.

---

## Delivery Method

GHL Conversation AI workflow — real automation, not a mockup. Wizard-of-Oz backend acceptable if needed to pass the credibility test.

---

## Scenario

An HVAC or plumbing contractor gets a new web lead. The lead submits a form or texts in. GHL triggers an automated AI conversation that:

1. Acknowledges immediately ("Thanks for reaching out to [COMPANY]...")
2. Qualifies the lead (service needed, location, urgency/timeline)
3. Either books a call slot or escalates to the contractor with a summary

The contractor never misses the lead. The conversation runs 24/7 without them.

---

## Credentials

All tokens stored in `.env` at repo root (gitignored, never committed).

| Variable | Description |
|----------|-------------|
| `GHL_AGENCY_TOKEN` | Agency PIT — location management only |
| `GHL_AGENCY_COMPANY_ID` | `Lrx3AfmHRi5cXS6N9iiQ` |
| `GHL_DEMO_LOCATION_ID` | `ALg2PWHg53TGuMy4rlPQ` — AI Business Lab Demo Account |
| `GHL_DEMO_TOKEN` | Demo sub-account PIT — full location access, use for all Experiment 001 build work |

---

## What Was Built

**GHL Sub-account:** AI Business Lab — Demo Account (`ALg2PWHg53TGuMy4rlPQ`)
**Demo contact:** Mike Thompson — simulated HVAC homeowner lead
**Conversation ID:** `VR2K377w1pWEwCJNt91t`
**Pipeline:** Lead Recovery Pipeline (`QnBh7eXPXpq0pHXEevOC`)
**Calendar:** Contractor Consultation (`ccRHQU68xlAvyotFX6e4`)
**Opportunity:** Mike Thompson — AC Repair, Stage: Booked

**Full conversation built (7 messages, SMS):**

1. Mike (inbound): "Hey I need someone to come look at my AC. Its not cooling the house."
2. AI (outbound): Immediate acknowledgment + first qualifying question (running but not cooling, or not running at all?)
3. Mike (inbound): "Its running but the house wont cool down. Its like 80 degrees in here"
4. AI (outbound): Diagnoses likely issue + asks urgency and location
5. Mike (inbound): "Started yesterday. Im in Peoria IL"
6. AI (outbound): Confirms coverage + offers same-day/next-day booking + gets buy-in
7. Mike (inbound): "Yeah that works great"
8. AI (outbound): Drops booking link, confirms next step

**What to show Ryan:** Open GHL > AI Business Lab Demo Account > Conversations > Mike Thompson. The full thread is there. Walk a contractor through it saying: "This is what happens the second a lead texts your business — day or night, while you're on a job."

---

## Wizard-of-Oz Elements

- **Conversation is pre-built** — in production this would be GHL Conversation AI (their "AI Employee" feature) responding dynamically. The demo shows the exact conversation flow a real AI would produce; the AI is simulated for Gate 1.
- **Booking link** — calendar is live but not connected to a real tech's schedule. Replace `[COMPANY NAME]` placeholder before showing to a real contractor.
- **Workflow automation** — GHL workflow (inbound SMS trigger → AI response) must be built in the GHL UI. API does not support workflow creation. See Production Setup section below.

---

## Production Setup (what turns this into a real product)

1. GHL Conversation AI bot configured in the sub-account UI (Settings > Conversation AI)
2. Workflow: Trigger = "Contact Created" or "Inbound SMS" → Action = "Conversation AI Reply"
3. Bot trained on: service types, coverage area, urgency questions, booking link for that contractor
4. Calendar connected to contractor's real availability

Estimated setup time per contractor: 45-60 min in GHL UI once template is standardized.

---

## Known Limitations

- "Contractor Consultation" calendar slug needs to resolve to a real booking page before going live
- `[COMPANY NAME]` placeholder must be swapped per client
- Workflow automation requires UI setup — not yet done in the demo account

---

## Gate 1 Credibility Review

**Ryan approval date:**
**Result:** Pass / Fail
**Notes:**
**Confidence Score (before/after):** 60% → _____%
