# Workflows

Workflows are sequences of agent tasks that accomplish a defined business outcome.

Agents do not have permanent jobs. Workflows require agents temporarily.

---

## Philosophy

Instead of maintaining a standing team of 15 agents, define workflows that pull the right agents for a specific task. When the workflow ends, agents return to dormant. Only the 3-agent core team stays permanently active.

This prevents agent sprawl. A roster of 15 agents sounds powerful but creates coordination overhead that exceeds the value. A roster of 3 agents plus on-demand workflows stays manageable indefinitely.

---

## Workflow anatomy

Every workflow document defines:

- **Goal:** What gets accomplished
- **Trigger:** What starts this workflow
- **Agents required:** Which agents are activated for this workflow
- **Sequence:** Step-by-step task order
- **Inputs:** What data or files the workflow needs
- **Outputs:** What gets committed to the repo when done
- **Success criteria:** How we know it worked
- **Ryan touchpoints:** Where Ryan approves before work continues

---

## Current workflows

| Workflow | File | Status | Trigger |
|----------|------|--------|---------|
| Validate Business Idea | `VALIDATE_BUSINESS_IDEA.md` | READY | Ryan selects a finalist idea |
| Design First Offer | `DESIGN_FIRST_OFFER.md` | NOT STARTED | Strategy decision made |
| Close First Client | `CLOSE_FIRST_CLIENT.md` | NOT STARTED | Offer defined and approved |
| Onboard First Client | `ONBOARD_FIRST_CLIENT.md` | NOT STARTED | Client signs |
| Monthly Business Review | `MONTHLY_REVIEW.md` | NOT STARTED | First revenue arrives |

---

## How to start a workflow

1. Chief of Staff identifies the trigger event in NEXT_ACTIONS.md
2. Chief of Staff opens the workflow document and reads Step 1
3. Activate only the agents listed in the workflow — no others
4. Each step's output is committed before the next step begins
5. Ryan touchpoints must be completed before the subsequent step
6. When the workflow ends, all temporarily activated agents return to dormant
7. Librarian records the workflow result in KNOWLEDGE_BASE.md
