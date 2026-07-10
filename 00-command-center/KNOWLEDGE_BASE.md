# Knowledge Base

**Maintained by:** Librarian
**Purpose:** Institutional memory for AI Business Lab. Experiments, decisions, failures, and lessons — recorded so the system improves over time.

---

## Index

| Date | Entry | Type |
|------|-------|------|
| 2026-07-09 | Repository initialized | Decision |
| 2026-07-09 | Track A research complete — 15 ideas scored | Experiment |
| 2026-07-09 | Track B research complete — 30 ideas scored | Experiment |
| 2026-07-09 | Agent library imported — 276 files | Decision |
| 2026-07-09 | Active roster reduced from 7 to 3 | Decision |

---

## Entries

### 2026-07-09 — Repository Initialized

**Type:** Decision
**Context:** Starting AI Business Lab as a GitHub-based operating system for building AI-assisted businesses.
**What happened:** Chose repo-as-office model. All agent communication happens through committed files, not conversation threads.
**What we learned:** Version control is the only durable communication channel for a multi-agent system. Anything not committed is lost.
**Applies to:** All future agent workflows.

---

### 2026-07-09 — Track A Research: 15 Founder-Leverage Ideas Scored

**Type:** Experiment
**Context:** First research pass on business ideas using Ryan's existing assets and expertise as inputs.
**What happened:** Top 5: AI Content Subscription (51/60), AI Local SEO Subscription (49.5/60), AI Lead Follow-Up (47.5/60), AI YouTube Scripts (47/60), AI Competitive Intelligence (45/60).
**What we learned:** All Track A ideas score moderate on business quality (3.5/5 average) when founder advantage is stripped out. Job risk is 2-3/5 for service-oriented ideas. The Local SEO Subscription carries the highest job risk of the top 5.
**Applies to:** Strategy selection decision. Any future idea scoring pass.

---

### 2026-07-09 — Track B Research: 30 Clean-Slate Ideas Scored

**Type:** Experiment
**Context:** Second research pass with founder history deliberately excluded. Ideas generated from scratch across 10 market categories.
**What happened:** Top 5: Job Description Bias Checker (54.5/60), ADA Compliance Monitoring (54/60), Privacy Policy Monitor (54/60), Contract Redline Summarizer (53.5/60), SOC 2 Template Pack (53.5/60). All score 4-5/5 on job risk.
**What we learned:** Business quality is materially higher when founder advantage is not a scoring criterion. Compliance and automation tools score highest on passivity and defensibility. Trade-off: Ryan has no distribution head start in these markets.
**Applies to:** Strategy selection. Any future idea in regulated markets.

---

### 2026-07-09 — Agent Library Imported

**Type:** Decision
**Context:** Imported 276 agent definitions from msitarzewski/agency-agents (MIT license) into the library.
**What happened:** 243 true agent definitions across 18 departments. 31 rated High relevance to AI Business Lab. 160 rated Low (game dev, GIS, healthcare, academic — not relevant to current work).
**What we learned:** A library without a registry becomes unsearchable. AGENT_REGISTRY.md is required. Activation should be workflow-driven, not standing roster.
**Applies to:** All future agent activation decisions.

---

### 2026-07-09 — Active Roster Reduced from 7 to 3

**Type:** Decision
**Context:** Initial PR activated 7 agents. Review identified this as over-hiring for Phase 1.
**What happened:** Reduced to 3-agent core team: Chief of Staff, Business Strategist, Project Manager. Librarian added as permanent knowledge role. Six agents deactivated to dormant.
**What we learned:** Activating agents before they have a defined task creates coordination overhead. The correct model is workflow-driven activation — agents are dormant until a workflow requires them.
**Applies to:** All future activation decisions. Agent limit during Phase 1 is 3 core + workflow-specific temporaries.
