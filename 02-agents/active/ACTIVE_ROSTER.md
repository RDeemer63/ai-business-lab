# Active Agent Roster

**Last updated:** 2026-07-09
**Current phase:** Phase 1 — Design the Company
**Active count:** 3 (limit: 15)
**Philosophy:** Hire for the current need, not the anticipated need. Dormant agents are available but not burning coordination overhead.

---

## Core Team (Always Active)

| Agent | File | Role | First Task |
|-------|------|------|------------|
| Chief of Staff | `custom/chief-of-staff.md` | Coordination, routing, command center | Maintain NEXT_ACTIONS.md, route tasks |
| Business Strategist | `active/business-strategist.md` | Strategy analysis, opportunity evaluation | Evaluate Strategy A vs. B vs. C |
| Project Manager | `custom/project-manager.md` | Keep work moving, track task status | Monitor agent queue, update task statuses |

Note: Chief of Staff, Project Manager, and Librarian live in `custom/` and are always considered active. They do not need to be moved to `active/`.

---

## Permanent Knowledge Role

| Agent | File | Role |
|-------|------|------|
| Librarian | `custom/librarian.md` | Institutional memory — records every experiment, decision, and lesson |

---

## Dormant (Available on Demand)

These agents are indexed in `AGENT_REGISTRY.md`. The Chief of Staff activates them for a specific workflow. They return to dormant when the workflow ends.

| Agent | Library Path | Activate When |
|-------|-------------|---------------|
| Offer & Lead Gen Strategist | `library/agency-agents/sales/sales-offer-lead-gen-strategist.md` | Offer is being designed |
| Pricing Analyst | `library/agency-agents/specialized/specialized-pricing-analyst.md` | Pricing decision is ready |
| Outbound Strategist | `library/agency-agents/sales/sales-outbound-strategist.md` | First client outreach begins |
| Proposal Strategist | `library/agency-agents/sales/sales-proposal-strategist.md` | First client call is booked |
| Customer Success Manager | `library/agency-agents/specialized/customer-success-manager.md` | First client signs |
| Trend Researcher | `library/agency-agents/product/product-trend-researcher.md` | New market research needed |
| SEO Specialist | `library/agency-agents/marketing/marketing-seo-specialist.md` | Strategy A confirmed |
| Email Marketing Strategist | `library/agency-agents/marketing/marketing-email-strategist.md` | First 5 clients signed |
| Financial Analyst | `library/agency-agents/finance/finance-financial-analyst.md` | First revenue arrives |

---

## Retired

None yet.

---

## Activation Rule

Agents are not activated individually. Workflows are activated. Each workflow names the agents it requires. Those agents are live for the duration of the workflow and return to dormant when it completes. See `03-workflows/` for defined workflows.
