# Chief Architect Briefing — 2026-07-10

---

## Current State

Experiment 001 (AI Lead Follow-Up Service) is in progress. Gate 1 passed today. The demo is live in a dedicated GHL sandbox sub-account — a full 7-message SMS qualification conversation for an HVAC contractor lead. Ryan's credibility review: "Pretty good." Confidence: 60% → 75%.

Gate 2 is next. Ryan runs 3 live contractor demos (screen-share), observes reactions, records verbatim answers. No engineering needed until Gate 2 results come back.

---

## Decisions Required

1. **Gate 2 interview guide** — built this session (6 capture points per demo). Does the format need any changes before Ryan uses it?
2. **Demo recording** — recommend Ryan record audio of Gate 2 demos for the Pattern Analyst. Should recording consent be a hard requirement or optional?
3. **A2P registration timing** — start now in parallel with Gate 2, or wait for Gate 3 confirmation first?

---

## Evidence Since Last Review

| Item | What it showed | File |
|------|---------------|------|
| GHL API investigation | Conversations AI config is UI-only — no public API for bot setup | `GATE_1_RESULT.md` |
| Gate 1 demo build | 7-message HVAC qualification conversation built and approved by Ryan | `DEMO_BUILD.md` |
| Technical assumption invalidated | Original plan was GHL native AI. Experiment found a better architecture: Claude webhook layer. Hypothesis unchanged. | `PARKING_LOT.md` |
| Constitutional rule | OPERATING_PRINCIPLES.md v1.1 — no principle without traceable evidence | `OPERATING_PRINCIPLES.md` |
| Confidence tracking formalized | Gate 1 entry now includes Before / After / Why it changed / Evidence | `EXPERIMENT_001.md` |

---

## Questions for Chief Architect

1. The Claude webhook architecture is parked as "AI Conversation Engine" capability. Correct framing? Should the parking lot entry reference Tulboxx portability more explicitly given that's a primary reason to build it properly?

2. Gate 2 is designed as observation, not selling. The interview guide has 6 capture points and a verbatim question that cannot be paraphrased. Is there anything the guide misses that you'd want captured from contractor conversations at this stage?

3. Confidence tracking is now logged per gate with Before / After / Why / Evidence. Over time this builds a learning history. Do you want us to also track confidence at the studio level — not just per experiment — as a separate metric?

---

## Recommended Reading Order

1. `04-experiments/experiment-001/GATE_1_RESULT.md` — what passed and why, A2P constraint, Gate 2 authorization
2. `04-experiments/experiment-001/GATE_2_INTERVIEW_GUIDE.md` — the 6-point observation framework for contractor demos
3. `00-command-center/PARKING_LOT.md` — AI Conversation Engine entry (renamed and expanded from Claude webhook layer)

---

## Expected Output

- Confirmation or revision of the Gate 2 interview guide before Ryan runs demos
- Ruling on A2P registration timing
- Any architectural input on the AI Conversation Engine capability framing before it graduates from the parking lot post-Gate-3
