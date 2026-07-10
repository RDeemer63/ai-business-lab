# Command Center — NEXT_ACTIONS.md

**Current Mission:** Build an autonomous venture studio that repeatedly discovers, validates, and launches businesses — each one requiring under 5 hours/week of Ryan's time after stabilization.

**Current Phase:** Phase 1 — Design the Studio

---

## This Week's Priority

Approve the Venture Studio Manifesto and run Experiment Zero.

Research is complete. Two idea tracks are documented. The studio architecture is built. The next step is not choosing a business — it is testing whether the studio can run a validation cycle without Ryan becoming the bottleneck.

See: `04-experiments/EXPERIMENT_ZERO.md`

---

## Open Decisions

| # | Decision | Owner | Status |
|---|----------|-------|--------|
| 1 | Approve VENTURE_STUDIO_MANIFESTO.md | Ryan | DONE — approved 2026-07-09 |
| 2 | Approve the PR (`feature/import-agent-library`) and merge | Ryan | DONE — merged 2026-07-09 |
| 3 | Approve VALIDATION_PLAN.md to advance Experiment Zero to Step 6 | Ryan | OPEN — plan at `04-experiments/experiment-zero/VALIDATION_PLAN.md` |

---

## Three Assumption Tests (replacing "validate 3 businesses")

We are not validating businesses. We are testing three assumptions.

**Assumption 1:** "Businesses with an urgent legal fear will buy a self-serve monitoring product without a sales call."
- Test vehicle: ADA Compliance Monitoring (Track B)
- Method: 20 cold emails with free scan results attached
- Signal: 3+ genuine replies expressing interest
- Also serves as Experiment Zero — the meta-test of the studio itself

**Assumption 2:** "Contractors will pay for AI to respond to leads they're already losing."
- Test vehicle: AI Lead Follow-Up Service (Track A)
- Method: Walk 3 contractors through a live GHL demo, ask for verbal commitment
- Signal: At least 1 asks "how do I sign up?" before the demo ends

**Assumption 3 (Experiment Zero):** "The studio can run a full validation cycle with under 2 hours of Ryan's time."
- Test vehicle: The studio's own process, run against Assumption 1
- KPI: Process quality, not market response
- See `04-experiments/EXPERIMENT_ZERO.md` for full definition

---

## Agent Queue

| Agent | Task | Status |
|-------|------|--------|
| Chief of Staff | Route Experiment Zero steps after Ryan approves Manifesto | WAITING ON RYAN |
| Business Strategist | Run Steps 1 and 3 of Experiment Zero (scoping + competitor analysis) | QUEUED — starts when Manifesto approved |
| Trend Researcher | Run Step 2 of Experiment Zero (market research — ADA monitoring) | QUEUED — activate for this workflow only |
| Newsletter Editor | Draft Issue 001 — "We Are Building an Autonomous Venture Studio" | QUEUED |
| Historian | Write decision record for venture studio reframe | QUEUED |

---

## Needs Ryan

- [ ] Read `00-command-center/VENTURE_STUDIO_MANIFESTO.md` — approve or amend before it becomes the constitutional document
- [ ] Merge PR #1 (`feature/import-agent-library`)
- [ ] Say "Start Experiment Zero" to begin the first validation cycle

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

### 2026-07-09 — Chief of Staff (Clean Slate Research)

**What I did:** Ran a second, fully independent research track with founder-history bias eliminated. Generated 30 business ideas across 10 categories without reference to Ryan's existing companies, industries, audiences, or software. Scored all 30 on 10 business-quality criteria (no founder advantage). Ran a separate Ryan fit analysis on the top 10. Wrote full profiles for all top 10. Created a combined comparison document synthesizing both tracks.

**What changed:**
- Created `01-business-ideas/CLEAN_SLATE_PIPELINE.md` — all 30 ideas scored; top 10 with full profiles including Ryan fit analysis; ideas 11-30 as a ranked scored table.
- Created `01-business-ideas/CLEAN_SLATE_TOP5.md` — readable brief on the top 5 clean-slate finalists, formatted identically to the Track A brief.
- Created `01-business-ideas/COMBINED_COMPARISON.md` — cross-track synthesis: normalized scores for both tracks, where they agree and diverge, recommended 3-test validation sequence, and an honest answer to whether the best opportunity is inside or outside Ryan's current expertise.

**What I recommend next:** Ryan reads `COMBINED_COMPARISON.md` before making any decision. It costs nothing to run all three validation tests simultaneously — the combined comparison recommends doing exactly that before choosing a track or strategy.

**Files touched:**
- `01-business-ideas/CLEAN_SLATE_PIPELINE.md` (created)
- `01-business-ideas/CLEAN_SLATE_TOP5.md` (created)
- `01-business-ideas/COMBINED_COMPARISON.md` (created)
- `00-command-center/NEXT_ACTIONS.md` (updated — this entry)

**Needs Ryan:** Read `COMBINED_COMPARISON.md`. The open decisions above remain unchanged — no decision should be made until Ryan reviews both tracks side by side.

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

---

### 2026-07-09 — Chief of Staff (Architecture Review)

**What I did:** Implemented pre-merge architectural improvements. Reduced active roster from 7 to 3. Added registry, principles, librarian, knowledge base, and first workflow definitions.

**What changed:**
- `02-agents/active/ACTIVE_ROSTER.md` — rewritten; 3-agent core team only; 6 agents returned to dormant
- `02-agents/active/` — 6 agents removed (originals remain in library/): customer-success-manager, offer-lead-gen-strategist, outbound-strategist, pricing-analyst, proposal-strategist, trend-researcher
- `02-agents/custom/librarian.md` — new permanent knowledge role created
- `02-agents/custom/project-manager.md` — new core team member created (based on library/project-management/project-manager-senior.md)
- `02-agents/AGENT_REGISTRY.md` — queryable agent metadata database created (10 agents evaluated)
- `00-command-center/OPERATING_PRINCIPLES.md` — 11-principle system constitution created
- `00-command-center/KNOWLEDGE_BASE.md` — institutional memory initialized with 5 entries
- `03-workflows/README.md` — workflow philosophy and index created
- `03-workflows/VALIDATE_BUSINESS_IDEA.md` — first defined workflow, ready to run
- `AGENTS.md` — updated to reflect new philosophy, directory structure, and core team

**What I recommend next:** Ryan merges the PR. The first workflow to run is VALIDATE_BUSINESS_IDEA — trigger it by selecting one idea from COMBINED_COMPARISON.md.

**Files touched:** All files listed above.

**Needs Ryan:** Merge the PR. Then select the first idea to validate from COMBINED_COMPARISON.md.

**Needs Ryan:** Review `02-agents/active/ACTIVE_ROSTER.md` and confirm the 7 activated agents before merging the PR. No decisions required — just a sanity check.

---

### 2026-07-09 — Chief of Staff (Venture Studio Reframe)

**What I did:** Implemented the strategic reframe from "build one business" to "autonomous venture studio." Created the manifesto, Intelligence Department (Historian, Pattern Analyst, Knowledge Curator), 09-lessons/ directory structure, Experiment Zero, department structure, and reframed the three validation tests as assumption tests.

**What changed:**
- `00-command-center/VENTURE_STUDIO_MANIFESTO.md` (created — constitutional document, pending Ryan approval)
- `02-agents/custom/historian.md` (created — records decisions and post-mortems)
- `02-agents/custom/pattern-analyst.md` (created — monthly pattern identification)
- `02-agents/custom/knowledge-curator.md` (created — keeps agent definitions current)
- `02-agents/departments/intelligence/README.md` (created)
- `02-agents/departments/research/README.md` (created)
- `02-agents/departments/operations/README.md` (created)
- `02-agents/departments/sales/README.md` (created)
- `09-lessons/` (created — 5 subdirectories: decisions, experiments, post-mortems, pattern-reports, prompt-quality)
- `04-experiments/EXPERIMENT_ZERO.md` (created — meta-experiment testing the studio's own process)
- `00-command-center/NEXT_ACTIONS.md` (updated — mission reframed, decisions updated, assumption-based test framing)

**What I recommend next:** Ryan reviews and approves VENTURE_STUDIO_MANIFESTO.md. Then merges the PR. Then says "Start Experiment Zero." The studio runs the first full validation cycle autonomously from there.

**Files touched:** All listed above.

**Needs Ryan:** Approve VENTURE_STUDIO_MANIFESTO.md. It is not in effect until Ryan reviews it.

---

### 2026-07-09 — Lead Engineer (Architecture Freeze v1.0)

**What I did:** Executed Architecture Freeze v1.0. Created 25 files across 8 new directories. All committed to `feature/import-agent-library` at commit 50f9a9e.

**What changed:**
- `10-architecture/ADR-0001-repository-as-organizational-state.md` (created)
- `10-architecture/ADR-0002-roles-defined-by-documents-not-models.md` (created)
- `00-command-center/ARCHITECTURE_FREEZE_v1.md` (created -- Three Laws, Architecture Budget, frozen structures)
- `00-command-center/PARKING_LOT.md` (created -- 5 seed entries: dashboard, orchestration, Intelligence Dept, weekly cadence, maturity levels)
- `00-command-center/CHIEF_ARCHITECT/` (5 files: README, DESIGN_PHILOSOPHY, QUESTIONS_I_ALWAYS_ASK, REVIEW_PROCESS, COMMON_FAILURE_PATTERNS)
- `00-command-center/LEAD_ENGINEER/` (5 files: README, ENGINEERING_PHILOSOPHY, IMPLEMENTATION_CHECKLIST, CODING_STANDARDS, DECISIONS_NOT_TO_BUILD)
- `00-command-center/FOUNDER/` (5 files: README, INVESTMENT_CRITERIA, KILL_CRITERIA, DECISION_RULES, RISK_TOLERANCE)
- `11-review/` (README + 5 subdirectories: pending/, completed/, architecture/, business/, engineering/)

**What I recommend next:**
1. Ryan reads and approves `00-command-center/VENTURE_STUDIO_MANIFESTO.md`
2. Ryan merges PR #1 (`feature/import-agent-library` -> main)
3. Ryan says "Start Experiment Zero"

**Files touched:** All 25 files listed above.

**Needs Ryan:** Approve manifesto. Merge PR #1. Say "Start Experiment Zero."

---

### 2026-07-09 — Lead Engineer (Receipt + Definition of Done patterns)

**Claimed:** Apply Open Engine implementation patterns (receipts, definition of done, stop conditions) to the workflow template and trail format — without changing the frozen architecture.

**Definition of Done:** AGENTS.md trail format and VALIDATE_BUSINESS_IDEA.md both updated with the three patterns. Committed and pushed.

**What I did:** Updated AGENTS.md trail format to require a "What I did NOT do and why" receipt field and explicit "Stop condition" field. Updated all five steps of VALIDATE_BUSINESS_IDEA.md with explicit Definition of Done and Stop Condition for each step.

**What I did NOT do and why:** Did not create a ticket queue or claim-lock system. No evidence of concurrent agent collision yet — that pattern waits for Parking Lot review. Did not write ADR-0003. The principle (work moves through state, not conversations) is already covered by ADR-0001; a new ADR needs a concrete decision gap to encode, not a restatement.

**Files touched:**
- `AGENTS.md`
- `03-workflows/VALIDATE_BUSINESS_IDEA.md`

**Stop condition (if any):** None — full scope completed.

**Needs Ryan:** None. Next action is still: approve manifesto, merge PR #1, say "Start Experiment Zero."

---

### 2026-07-09 — Lead Engineer (Experiment Zero: Steps 2-4)

**Claimed:** Run Experiment Zero Steps 2-4 for ADA Compliance Monitoring. Produce validation plan for Ryan's Step 5 approval.

**Definition of Done:** MARKET_RESEARCH.md, COMPETITOR_ANALYSIS.md, OFFER_DESIGN.md, and VALIDATION_PLAN.md all exist in `04-experiments/experiment-zero/` with specific, evidence-based content. RYAN_TIME_LOG.md template created. EXPERIMENT_ZERO.md status updated.

**What I did:** Wrote MARKET_RESEARCH.md with ADA lawsuit data (4,600+ federal suits in 2023, Seyfarth Shaw), buyer profile (5-50 employee businesses in restaurant/retail/healthcare/legal), and pain evidence (Robles v. Domino's, Winn-Dixie, serial plaintiff mechanics, $25,000-$50,000 average settlement). Wrote COMPETITOR_ANALYSIS.md covering 7 competitors with real pricing: accessiBe ($490/yr overlay), AudioEye ($49/mo overlay), UserWay ($49/mo overlay), Pope Tech ($20-150/mo monitoring), Deque axe Monitor ($279/mo), Siteimprove ($250+/mo), BoIA ($300-1,000/mo). Identified the positioning gap: monitoring-only at $99/month with plain-language reports does not exist in this market. Wrote OFFER_DESIGN.md with offer name (ClearPath ADA Monitor), two tiers ($99/mo Solo, $179/mo Multi), plain-language report differentiator, and free-scan acquisition mechanic. Wrote VALIDATION_PLAN.md targeting owners/managers at 5-50 employee businesses in high-lawsuit industries via 100 cold emails with personalized free scan reports over 7 days. Success = 3+ genuine interest replies.

**What I did NOT do and why:** Did not build any scanning infrastructure, email system, or landing page. The validation plan calls for manual execution first — building before validation signal is the failure mode the studio exists to prevent. Did not select specific prospects or write the email — that is Step 6, which requires Ryan's approval of this plan first.

**Files touched:**
- `04-experiments/experiment-zero/MARKET_RESEARCH.md` (created)
- `04-experiments/experiment-zero/COMPETITOR_ANALYSIS.md` (created)
- `04-experiments/experiment-zero/OFFER_DESIGN.md` (created)
- `04-experiments/experiment-zero/VALIDATION_PLAN.md` (created — pending Ryan approval)
- `04-experiments/experiment-zero/RYAN_TIME_LOG.md` (created — template for Ryan to fill in)
- `04-experiments/EXPERIMENT_ZERO.md` (updated — status changed to IN PROGRESS)
- `00-command-center/NEXT_ACTIONS.md` (updated — Open Decisions table updated, this entry added)

**Stop condition (if any):** None encountered. The market research is substantive. The offer is differentiated. The validation plan is specific. Ready for Ryan's review.

**Needs Ryan:**
- [ ] Read `04-experiments/experiment-zero/VALIDATION_PLAN.md` and approve or amend — this is Step 5. Approval authorizes Step 6 (outreach message design).
- [ ] Log your time for Step 1 (idea selection) in `04-experiments/experiment-zero/RYAN_TIME_LOG.md`
- [ ] One pre-test action before Step 6: run one sample scan on any business website using the free axe DevTools Chrome extension or Google Lighthouse, screenshot the results, and confirm the format is usable as a report. This takes 10 minutes and confirms the mechanic works before we design the email around it.
