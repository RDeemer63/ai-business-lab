# Active Agent Roster

**Last updated:** 2026-07-09
**Current phase:** Phase 1 — Design the Company
**Active count:** 10 (limit: 15)

Agents in `02-agents/custom/` are always considered active — they are AI Business Lab-specific.
Agents in `02-agents/active/` are imported from the library and approved for current use.

---

## Custom Agents (Always Active)

| Agent | File | First Task | Scope |
|-------|------|------------|-------|
| Chief of Staff | `custom/chief-of-staff.md` | Maintain NEXT_ACTIONS.md, route tasks, write weekly status | All coordination and routing |
| Business Research Agent | `custom/business-research.md` | Score business ideas and validate finalists | Idea evaluation and market research |
| Newsletter Editor | `custom/newsletter-editor.md` | Draft Issue 001 — "Building an AI-Run Business From Scratch" | Newsletter drafts and content documentation |

---

## Active (From Library)

These 7 agents were activated for Phase 1. Each has a defined first task and a scope boundary.

### Business Strategist
- **Source:** `library/agency-agents/specialized/business-strategist.md`
- **Activated:** 2026-07-09
- **Why now:** Phase 1 requires evaluating three launch strategies (A, B, C). This agent provides competitive analysis and market entry framing.
- **First task:** Evaluate Strategy A vs. Strategy B vs. Strategy C. Produce a one-page argument for each, then a recommended path.
- **Scope:** Strategy analysis and competitive positioning only. Does not replace Business Research Agent for idea scoring.
- **Needs customization:** No — can be used as-is for strategy analysis. If contractor-specific context is needed, add it in the task brief.

### Offer & Lead Gen Strategist
- **Source:** `library/agency-agents/sales/sales-offer-lead-gen-strategist.md`
- **Activated:** 2026-07-09
- **Why now:** Whichever strategy Ryan picks, a defined offer is required before the first client conversation. This agent designs the offer and lead magnet.
- **First task:** Draft the first offer for Strategy A (content/SEO subscription for contractors). Define the lead magnet, the entry offer, and the value ladder.
- **Scope:** Offer design and lead generation architecture. Does not run outbound — that is Outbound Strategist.
- **Needs customization:** No — but task briefs must include the contractor audience context.

### Trend Researcher
- **Source:** `library/agency-agents/product/product-trend-researcher.md`
- **Activated:** 2026-07-09
- **Why now:** Market validation is Phase 1's core research task. Trend Researcher identifies what contractors are spending money on right now and how demand is shifting.
- **First task:** Research the local contractor market for AI-powered services — what are contractors currently buying, what are they complaining about, and what does competitor pricing look like for content, SEO, and lead follow-up services.
- **Scope:** Market intelligence only. Does not score or rank ideas — that stays with Business Research Agent.
- **Needs customization:** No for initial use.

### Outbound Strategist
- **Source:** `library/agency-agents/sales/sales-outbound-strategist.md`
- **Activated:** 2026-07-09
- **Why now:** Reaching first clients requires a systematic prospecting approach. Activated now so the outbound plan is ready when the offer is defined.
- **First task:** (On hold until offer is defined.) Design a 10-touch outbound sequence for reaching HVAC and plumbing contractors in Ryan's existing network. Include channel, message angle, and personalization approach.
- **Scope:** Prospecting sequence design only. Does not send messages — Ryan sends them.
- **Needs customization:** No. Task briefs must include ICP description and offer once finalized.

### Pricing Analyst
- **Source:** `library/agency-agents/specialized/specialized-pricing-analyst.md`
- **Activated:** 2026-07-09
- **Why now:** Pricing the first offer is a Phase 1 decision. Before the first client conversation, the price tier and value framing must be locked.
- **First task:** Analyze the pricing for an AI content subscription for contractors. Compare competitor rates, model margin at $297 vs. $497 vs. $750/month, and recommend the launch price with rationale.
- **Scope:** Pricing analysis and recommendation only. Does not finalize pricing — Ryan approves.
- **Needs customization:** No.

### Proposal Strategist
- **Source:** `library/agency-agents/sales/sales-proposal-strategist.md`
- **Activated:** 2026-07-09
- **Why now:** The first client conversations will require a proposal. Having a polished, consistent proposal template ready before outreach starts improves close rate.
- **First task:** Build a proposal template for the AI local SEO or content subscription offer. Should convert a discovery call into a signed client.
- **Scope:** Proposal writing and win narrative. Does not run outreach or pricing decisions.
- **Needs customization:** No for initial template. Will need contractor-specific voice and offer details once finalized.

### Customer Success Manager
- **Source:** `library/agency-agents/specialized/customer-success-manager.md`
- **Activated:** 2026-07-09
- **Why now:** Month 2 retention is where this business lives or dies. Having an onboarding and health-check framework ready before the first client signs prevents reactive firefighting.
- **First task:** Design the client onboarding checklist for a content subscription client. Cover first 30, 60, and 90 days. Define what a "healthy" client looks like vs. churn risk.
- **Scope:** Client onboarding, health scoring, and renewal. Does not handle sales or proposal writing.
- **Needs customization:** No for initial framework. Will evolve as client data accumulates.

---

## Retired

None yet.

---

## Activation Queue (Pending Ryan Decision)

These agents are in the library, rated HIGH, and ready to activate when the phase advances:

| Agent | Library Path | Activate When |
|-------|-------------|---------------|
| SEO Specialist | `library/agency-agents/marketing/marketing-seo-specialist.md` | Strategy A confirmed — will support Throttled Up delivery quality |
| Email Marketing Strategist | `library/agency-agents/marketing/marketing-email-strategist.md` | First 5 clients signed — build nurture and retention sequences |
| Financial Analyst | `library/agency-agents/finance/finance-financial-analyst.md` | First revenue — model path to $10k MRR |
| Analytics Reporter | `library/agency-agents/support/support-analytics-reporter.md` | First revenue — build MRR and churn tracking dashboard |
| Multi-Agent Systems Architect | `library/agency-agents/engineering/engineering-multi-agent-systems-architect.md` | Phase 3 — when agent coordination needs formal design |
