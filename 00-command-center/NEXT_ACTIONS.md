# Command Center — NEXT_ACTIONS.md

**Current Mission:** Build a $5k–$10k/month AI-assisted business with under 5 hours/week of human work.

**Current Phase:** Phase 1 — Design the Company

---

## This Week's Priority

Ryan reviews the top 5 finalists and selects a launch strategy.

Research is complete. The pipeline has 15 scored ideas. The top 5 are documented with full trade-off analysis. The decision brief is in `01-business-ideas/TOP5_DECISION_BRIEF.md`.

---

## Open Decisions

| # | Decision | Owner | Status |
|---|----------|-------|--------|
| 1 | Which launch strategy: A (content/SEO subscription now), B (build lead follow-up first), or C (run sprints to fund and inform first)? | Ryan | OPEN |
| 2 | After choosing strategy: which contractor problem does Ryan's existing network mention most — getting found, responding to leads, or tracking competitors? | Ryan | OPEN |
| 3 | Should Finalist 3 (Lead Follow-Up) be built as a bundled add-on or as the standalone first product? | Ryan | OPEN — depends on Decision 1 |

---

## Agent Queue

| Agent | Task | Status |
|-------|------|--------|
| Newsletter Editor | Draft Issue 001 — "We Are Building an AI-Run Business From Scratch" | QUEUED |
| Business Research Agent | Standby — ready to do deep-dive research on whichever finalist Ryan selects | ON HOLD |
| Chief of Staff | After Ryan chooses a strategy, update this file and assign Phase 2 tasks | WAITING ON RYAN |
| Business Strategist (library) | Evaluate Strategy A vs. B vs. C — produce one-page argument for each | QUEUED — activate after Ryan's strategy decision |
| Offer & Lead Gen Strategist (library) | Draft first offer and lead magnet — activate once strategy is confirmed | QUEUED |
| Pricing Analyst (library) | Analyze $297 vs. $497 vs. $750/month pricing for content subscription | QUEUED |

---

## Needs Ryan

- [ ] Read `01-business-ideas/TOP5_DECISION_BRIEF.md`
- [ ] Choose a launch strategy (A, B, or C) from the decision brief
- [ ] Answer: which problem do contractors in your network complain about most?

---

## Scoring Framework (Updated)

Rate each idea 1–5 on 10 criteria. Four criteria weighted at 1.5x:

| Criterion | Weight | Description |
|-----------|--------|-------------|
| C1 Startup cost | 1x | 5 = near zero |
| C2 AI automation potential | 1.5x | 5 = almost fully automated |
| C3 Speed to first dollar | 1.5x | 5 = first sale within 2 weeks |
| C4 MRR potential | 1x | 5 = $10k+/month ceiling |
| C5 Competition | 1x | 5 = low competition |
| C6 Difficulty | 1x | 5 = easy to execute |
| C7 Scalability | 1x | 5 = scales without Ryan |
| C8 Founder advantage | 1.5x | 5 = Ryan has unique edge no competitor has |
| C9 CS burden | 1x | 5 = very low client service burden |
| C10 Dependence on Ryan | 1.5x | 5 = delivery requires zero Ryan involvement |

**Weighted total = (C1+C4+C5+C6+C7+C9) + (C2+C3+C8+C10) × 1.5**
Max possible: 60

---

## Pipeline Summary

| Rank | Idea | Score |
|------|------|-------|
| 1 | AI Content Subscription (GBP + Blog + Social) | 51 |
| 2 | AI Local SEO Subscription (Throttled Up Productized) | 49.5 |
| 3 | AI Lead Follow-Up Service (GHL-Based) | 47.5 |
| 4 | AI YouTube Script + Short-Form Video System | 47 |
| 5 | AI Competitive Intelligence Reports | 45 |
| 6 | AI Bid/Proposal Optimization (Tulboxx-Adjacent) | 44.5 |
| 7 | AI Reputation Management Subscription | 44 |
| 8 | Tulboxx White-Label / Reseller | 44 |
| 9 | White-Label AI Marketing System for Agencies | 44 |
| 10 | Trades Newsletter with Paid Tier + Sponsorships | 43 |
| 11 | Niche Affiliate Media Site | 41 |
| 12 | Outta the Weeds Digital Course + Paid Community | 40.5 |
| 13 | OTW Framework Licensing to Business Coaches | 39 |
| 14 | Done-in-a-Day AI Implementation Sprint | 38.5 |
| 15 | Trades Business OS — GHL Snapshot + Setup | 37.5 |

---

## Activity Log

### 2026-07-09 — Claude Code

**What I did:** Set up initial repo structure — README, AGENTS.md, CLAUDE.md, command center, all three starter agent files, and business idea template.

**What changed:** Repository scaffolded from scratch.

**What I recommend next:** Ryan creates a GitHub repo at github.com/new, pushes this folder, then assigns the first task to Business Research Agent via NEXT_ACTIONS.md Agent Queue.

**Files touched:** All initial files.

**Needs Ryan:** Business model decision (see Open Decisions above).

---

### 2026-07-09 — Chief of Staff

**What I did:** Researched, scored, and documented all 15 business ideas against a 10-criterion weighted scoring framework. Identified the top 5 finalists. Wrote the decision brief comparing finalists and framing the launch strategy choice. Updated the command center to reflect research completion.

**What changed:**
- Created `01-business-ideas/IDEA_PIPELINE.md` — all 15 ideas scored and sorted highest to lowest. Each includes full scoring table, customer, problem, offer, pricing, revenue math, startup time, human work before and after stabilization, AI agent tasks, largest risk, 7-day validation test, and a skeptic's note.
- Created `01-business-ideas/TOP5_DECISION_BRIEF.md` — summaries of each finalist, comparison table, core trade-offs, bundle opportunities, and the exact decision Ryan needs to make.
- Updated `00-command-center/NEXT_ACTIONS.md` — open decisions and agent queue updated to reflect research complete status. Pipeline summary table added.

**What I recommend next:** Ryan reads the decision brief (not the pipeline — the brief). Then answers the three open decisions above. Once a strategy is chosen, Phase 2 begins: build the offer, define the sales process, and close the first client.

**Files touched:**
- `01-business-ideas/IDEA_PIPELINE.md` (created)
- `01-business-ideas/TOP5_DECISION_BRIEF.md` (created)
- `00-command-center/NEXT_ACTIONS.md` (updated)

**Needs Ryan:** Choose launch strategy A, B, or C from the decision brief.

---

### 2026-07-09 — Chief of Staff (Agent Library Import)

**What I did:** Cloned the msitarzewski/agency-agents repository. Restructured `02-agents/` into four subdirectories (library/, active/, custom/, retired/). Moved our three custom agents to custom/ with git history preserved. Imported all 276 upstream agent files. Created AGENT_INDEX.md covering every agent with relevance ratings. Created SELECTION_GUIDE.md with full lifecycle procedures. Activated 7 library agents for Phase 1. Updated the active roster.

**What changed:**
- `02-agents/` restructured — four subdirectories created: library/, active/, custom/, retired/
- `02-agents/custom/` — chief-of-staff.md, business-research.md, newsletter-editor.md moved here (git history preserved)
- `02-agents/library/agency-agents/` — 276 files imported from upstream (all directories and files preserved as-is)
- `02-agents/library/AGENT_INDEX.md` — created; covers all 276 files, grouped by department, rated High/Medium/Low for AI Business Lab relevance, overlap flags documented
- `02-agents/library/SELECTION_GUIDE.md` — created; full search, evaluate, customize, activate, and retire procedures; activation limit set at 15
- `02-agents/active/ACTIVE_ROSTER.md` — created; 10 active agents listed (3 custom + 7 library); activation queue for Phase 2 included
- `02-agents/active/` — 7 library agents copied here: business-strategist, offer-lead-gen-strategist, trend-researcher, outbound-strategist, pricing-analyst, proposal-strategist, customer-success-manager
- `vendor-licenses/agency-agents-LICENSE` — MIT license from upstream preserved verbatim
- `00-command-center/NEXT_ACTIONS.md` — Agent Queue updated with 3 library agent tasks queued

**What I recommend next:** Ryan reads ACTIVE_ROSTER.md (under 2 pages) to confirm the 7 activated agents make sense before merging the PR. Once the PR is merged, the first tasks to assign are: Pricing Analyst on the $297/$497/$750 analysis, and Business Strategist on the A/B/C strategy evaluation — both can run in parallel while Ryan makes the strategy decision.

**Files touched:**
- `02-agents/custom/chief-of-staff.md` (moved)
- `02-agents/custom/business-research.md` (moved)
- `02-agents/custom/newsletter-editor.md` (moved)
- `02-agents/library/agency-agents/` (276 files created)
- `02-agents/library/AGENT_INDEX.md` (created)
- `02-agents/library/SELECTION_GUIDE.md` (created)
- `02-agents/active/ACTIVE_ROSTER.md` (created)
- `02-agents/active/` (7 agent files added)
- `vendor-licenses/agency-agents-LICENSE` (created)
- `00-command-center/NEXT_ACTIONS.md` (updated)

**Needs Ryan:** Review `02-agents/active/ACTIVE_ROSTER.md` and confirm the 7 activated agents before merging the PR. No decisions required — just a sanity check.
