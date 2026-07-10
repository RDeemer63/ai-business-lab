# Experiment Zero — The Venture Studio Test

**Status:** COMPLETE — Assumption 3 validated (planning phase). Business not pursued.
**Type:** Meta-experiment (tests the organization, not a market)
**Date defined:** 2026-07-09

---

## Question

Can our AI organization take a business idea from concept to a validated go/no-go recommendation — without Ryan becoming the bottleneck?

---

## Why This Is the First Experiment

Before testing whether any specific business works, we need to know whether the machine that evaluates and validates businesses works. If the machine is broken, the market results are meaningless. If the machine works, every future experiment is faster and cheaper.

This experiment answers a different question than all others. Most experiments ask: "Will the market buy this?" This one asks: "Can the studio do its job?"

---

## What We Are Testing

Not: "Will people buy ADA compliance monitoring?"

We are testing: "Can the studio run a full validation cycle with under 2 hours of Ryan's time?"

---

## Process

Eight steps. Each step has a defined owner, defined output file, and a Ryan touchpoint flag.

| Step | Task | Owner | Ryan required? |
|------|------|-------|----------------|
| 1 | Idea selection and scoping | Business Strategist + Chief of Staff | Yes — final selection |
| 2 | Market research | Trend Researcher + Business Research Agent | No |
| 3 | Competitor analysis | Business Strategist | No |
| 4 | Offer design | Offer & Lead Gen Strategist | No |
| 5 | Validation plan | Chief of Staff | Yes — approve before Step 6 |
| 6 | Outreach message design | Outbound Strategist | Yes — approve before sending |
| 7 | Results documentation | Librarian + Historian | No |
| 8 | Go/no-go recommendation | Chief of Staff | Yes — review final recommendation |

Ryan touches Steps 1, 5, 6, and 8. Target: under 30 minutes per touchpoint, under 2 hours total.

---

## KPIs

| Metric | Target | Actual (fill in after) |
|--------|--------|----------------------|
| Steps completed without Ryan | 6 of 8 | Steps 2-4 ran without Ryan. Steps 1, 5, 6 required Ryan input. Steps 7-8 not reached. |
| Ryan's total time for the cycle | Under 2 hours | Not measured — execution phase not run. Planning cycle estimated at 1h45m after v3 workflow redesign. |
| Time from idea selection to recommendation | Under 7 days | Planning cycle: 1 day. Execution not run. |
| Steps with documented output files | 8 of 8 | 6 of 8 steps have output files. Steps 7-8 not reached. |
| Knowledge base entries created | At least 3 | 3 lesson files: STAGE_GATE_LESSONS.md, POST_MORTEM.md, RETROSPECTIVE.md |

---

## The Idea to Test

ADA Website Compliance Monitoring (Track B, Finalist 2 from `01-business-ideas/CLEAN_SLATE_TOP5.md`).

Reasons for this selection:
- No distribution advantage from Ryan's existing network — tests the machine, not Ryan's relationships
- Cold email hook is fully specifiable in advance
- Go/no-go signal is clear within 7 days
- Ryan fit score is high enough (15/20) that the idea is plausible, without being so familiar that Ryan shortcuts the process

---

## What Ryan Does

- Step 1: Selects this idea as the Experiment Zero subject (already done by reading this file)
- Step 5: Reviews and approves the validation plan before outreach is designed
- Step 6: Reviews and approves the outreach message before it is sent
- Step 6 (execution): Sends the emails — this action stays human in Phase 1
- Step 8: Reviews the go/no-go recommendation and decides whether to pursue

Everything between those touchpoints runs without Ryan.

---

## What Success Looks Like

The machine produces a go/no-go recommendation that Ryan can act on, and Ryan spent fewer than 2 hours total across all touchpoints.

Whether the market says yes or no to ADA monitoring is secondary. The primary result is whether the studio ran the cycle correctly.

---

## What Failure Looks Like

- Ryan spent more than 2 hours total
- A step stalled because no agent owned it
- The recommendation was delivered without documented evidence in the output files
- Ryan had to do research or drafting that the agents should have done

---

## Output Files

All output files go in `04-experiments/experiment-zero/`:

| File | Owner | Content |
|------|-------|---------|
| VALIDATION_PLAN.md | Chief of Staff | Full 7-day test plan, success metric, target channels |
| MARKET_RESEARCH.md | Trend Researcher + Business Research Agent | Market size, buyer profile, pain evidence |
| COMPETITOR_ANALYSIS.md | Business Strategist | Direct competitors, pricing, positioning gaps |
| OFFER_DESIGN.md | Offer & Lead Gen Strategist | Exact offer, price, value proposition |
| OUTREACH_DRAFT.md | Outbound Strategist | Email subject, body, follow-up sequence |
| RESULT.md | Librarian | Raw results: responses received, interest level, conversions |
| RYAN_TIME_LOG.md | Ryan (self-reported) | Each touchpoint: which step, what Ryan did, how long it took |

Post-experiment:
- `09-lessons/experiments/EXPERIMENT_ZERO_SUMMARY.md` — Librarian writes after results are in

---

## Experiment Scorecard

| Metric | Value |
|--------|-------|
| Experiment number | 000 |
| Outcome | Assumption 3 validated (planning phase). Business not pursued. |
| Planning cycle duration | 1 day |
| Documents produced | 12 |
| Review cycles | 3 (v1 → v2 → v3 validation plan) |
| Stage Gate blocks | 1 (KPI shift caught and resolved) |
| Workflow improvements | 2 (agent-prepared drafts; full funnel tracking) |
| Lessons filed | 3 (STAGE_GATE_LESSONS.md, POST_MORTEM.md, RETROSPECTIVE.md) |
| Architectural changes | 0 (Architecture Freeze held) |
| Businesses validated | 0 |
| Assumption 3 validated | Probably — with evidence from the planning phase |
| Organization improved | YES |

---

## Post-Experiment Record

Full record in `09-lessons/experiment-zero/`:
- POST_MORTEM.md — what happened, what the review caught, what changed
- RETROSPECTIVE.md — seven questions, honest answers
- STAGE_GATE_LESSONS.md — KPI defense rule, first organizational lesson
