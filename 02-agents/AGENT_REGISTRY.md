# Agent Registry

**Maintained by:** Librarian + Chief of Staff
**Purpose:** Queryable metadata for all evaluated agents. The Chief of Staff queries this before activating any agent.
**Last updated:** 2026-07-09

---

## How to query this registry

Before activating any agent:
1. Identify the task that needs to be done.
2. Search this registry by department or capability keyword.
3. Check status: Active = has a defined task now. Dormant = available on demand. Retired = do not reactivate without good reason.
4. If no match found here, search `02-agents/library/AGENT_INDEX.md` for unevaluated library agents.

---

## Registry

### Chief of Staff
| Field | Value |
|-------|-------|
| id | chief-of-staff |
| status | active |
| department | Operations |
| role | Coordinator |
| created_by | AI Business Lab |
| source | custom |
| file | 02-agents/custom/chief-of-staff.md |
| requires | File access, NEXT_ACTIONS.md |
| can_call | Any agent |
| reports_to | Ryan |
| approval_level | High — routes all decisions |
| cost_estimate | Low |
| quality | validated |
| times_used | 3 |
| rating | 5/5 |
| last_review | 2026-07-09 |
| notes | Core permanent role. Manages all coordination and routing. |

---

### Librarian
| Field | Value |
|-------|-------|
| id | librarian |
| status | active |
| department | Knowledge |
| role | Memory Keeper |
| created_by | AI Business Lab |
| source | custom |
| file | 02-agents/custom/librarian.md |
| requires | File access, git log access |
| can_call | Chief of Staff (escalations only) |
| reports_to | Chief of Staff |
| approval_level | Low — records, does not decide |
| cost_estimate | Low |
| quality | untested |
| times_used | 0 |
| rating | -- |
| last_review | 2026-07-09 |
| notes | Permanent role. Maintains KNOWLEDGE_BASE.md. Critical for long-term system value. |

---

### Project Manager
| Field | Value |
|-------|-------|
| id | project-manager |
| status | active |
| department | Operations |
| role | Task Tracker |
| created_by | AI Business Lab |
| source | custom (based on library/project-management/project-manager-senior.md) |
| file | 02-agents/custom/project-manager.md |
| requires | File access, NEXT_ACTIONS.md |
| can_call | Any agent |
| reports_to | Chief of Staff |
| approval_level | Low — tracks, does not decide |
| cost_estimate | Low |
| quality | untested |
| times_used | 0 |
| rating | -- |
| last_review | 2026-07-09 |
| notes | Keeps task queue moving. No task older than 48h without status update. |

---

### Business Strategist
| Field | Value |
|-------|-------|
| id | business-strategist |
| status | active |
| department | Strategy |
| role | Analyst |
| created_by | Agency Agents (msitarzewski) |
| source | upstream |
| file | 02-agents/active/business-strategist.md |
| requires | Web search, file access |
| can_call | Pricing Analyst, Trend Researcher |
| reports_to | Chief of Staff |
| approval_level | Medium |
| cost_estimate | Medium |
| quality | unknown |
| times_used | 0 |
| rating | -- |
| last_review | 2026-07-09 |
| notes | First task: evaluate Strategy A vs. B vs. C from COMBINED_COMPARISON.md. |

---

### Offer & Lead Gen Strategist
| Field | Value |
|-------|-------|
| id | offer-lead-gen-strategist |
| status | dormant |
| department | Sales |
| role | Offer Designer |
| created_by | Agency Agents (msitarzewski) |
| source | upstream |
| file | 02-agents/library/agency-agents/sales/sales-offer-lead-gen-strategist.md |
| requires | Web search |
| can_call | Pricing Analyst, Copywriter |
| reports_to | Chief of Staff |
| approval_level | Medium |
| cost_estimate | Low |
| quality | unknown |
| times_used | 0 |
| rating | -- |
| last_review | 2026-07-09 |
| notes | Activate when: offer is being designed after strategy decision. |

---

### Pricing Analyst
| Field | Value |
|-------|-------|
| id | pricing-analyst |
| status | dormant |
| department | Strategy |
| role | Pricing Specialist |
| created_by | Agency Agents (msitarzewski) |
| source | upstream |
| file | 02-agents/library/agency-agents/specialized/specialized-pricing-analyst.md |
| requires | Web search, market data |
| can_call | Business Strategist |
| reports_to | Chief of Staff |
| approval_level | Medium |
| cost_estimate | Low |
| quality | unknown |
| times_used | 0 |
| rating | -- |
| last_review | 2026-07-09 |
| notes | Activate when: pricing decision is ready. Do not activate before offer is defined. |

---

### Outbound Strategist
| Field | Value |
|-------|-------|
| id | outbound-strategist |
| status | dormant |
| department | Sales |
| role | Prospecting Specialist |
| created_by | Agency Agents (msitarzewski) |
| source | upstream |
| file | 02-agents/library/agency-agents/sales/sales-outbound-strategist.md |
| requires | Web search |
| can_call | Proposal Strategist |
| reports_to | Chief of Staff |
| approval_level | High — all outbound messages require Ryan approval before sending |
| cost_estimate | Low |
| quality | unknown |
| times_used | 0 |
| rating | -- |
| last_review | 2026-07-09 |
| notes | Activate when: first client outreach begins. All messages Ryan-approved before sending. |

---

### Proposal Strategist
| Field | Value |
|-------|-------|
| id | proposal-strategist |
| status | dormant |
| department | Sales |
| role | Proposal Writer |
| created_by | Agency Agents (msitarzewski) |
| source | upstream |
| file | 02-agents/library/agency-agents/sales/sales-proposal-strategist.md |
| requires | File access |
| can_call | Pricing Analyst |
| reports_to | Chief of Staff |
| approval_level | Medium |
| cost_estimate | Low |
| quality | unknown |
| times_used | 0 |
| rating | -- |
| last_review | 2026-07-09 |
| notes | Activate when: first client call is booked. |

---

### Customer Success Manager
| Field | Value |
|-------|-------|
| id | customer-success-manager |
| status | dormant |
| department | Operations |
| role | Client Success |
| created_by | Agency Agents (msitarzewski) |
| source | upstream |
| file | 02-agents/library/agency-agents/specialized/customer-success-manager.md |
| requires | File access, CRM data |
| can_call | Chief of Staff |
| reports_to | Chief of Staff |
| approval_level | Medium |
| cost_estimate | Low |
| quality | unknown |
| times_used | 0 |
| rating | -- |
| last_review | 2026-07-09 |
| notes | Activate when: first client signs. Month 2 retention is the primary concern. |

---

### Trend Researcher
| Field | Value |
|-------|-------|
| id | trend-researcher |
| status | dormant |
| department | Product |
| role | Market Researcher |
| created_by | Agency Agents (msitarzewski) |
| source | upstream |
| file | 02-agents/library/agency-agents/product/product-trend-researcher.md |
| requires | Web search |
| can_call | Business Strategist |
| reports_to | Chief of Staff |
| approval_level | Low |
| cost_estimate | Medium |
| quality | unknown |
| times_used | 0 |
| rating | -- |
| last_review | 2026-07-09 |
| notes | Activate for new market research. Not needed until Phase 2. |
