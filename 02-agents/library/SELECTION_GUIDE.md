# Agent Selection Guide

**Audience:** Chief of Staff
**Purpose:** How to search, evaluate, customize, activate, and retire agents from the library.

---

## The Activation Limit

No more than 15 agents in `02-agents/active/` at any time.

Beyond 15, coordination overhead exceeds the value. The Chief of Staff cannot track agent outputs, route tasks effectively, or maintain NEXT_ACTIONS.md clearly when the roster is too large. When the limit is reached, an agent must be retired before a new one can be activated.

The current limit applies to all agents across custom/ and active/ combined.

---

## 1. How to Search

Before activating any agent, search the library first. Never build a custom agent if a library agent covers the need adequately.

**Search by task type:**
Open `AGENT_INDEX.md`. Use the department groupings and the Relevance column (High / Medium / Low) as your first filter. High-relevance agents have been evaluated for AI Business Lab specifically.

**Search by keyword:**
Look for agents whose "Primary purpose" or "Expected outputs" match your task. Common tasks and where to find them:

| Task | Look in |
|------|---------|
| Pricing the offer | Specialized: Pricing Analyst |
| Designing the offer and lead magnet | Sales: Offer & Lead Gen Strategist |
| Writing a sales proposal | Sales: Proposal Strategist |
| Reaching first clients | Sales: Outbound Strategist, Sales Outreach |
| Market research | Product: Trend Researcher, Specialized: Business Strategist |
| Writing content | Marketing: Content Creator, Book Co-Author |
| SEO analysis | Marketing: SEO Specialist |
| Email sequences | Marketing: Email Marketing Strategist |
| Financial tracking | Finance: Financial Analyst, Support: Finance Tracker |
| Client retention | Specialized: Customer Success Manager |
| Code review | Engineering: Code Reviewer |
| Building AI pipelines | Engineering: AI Engineer, Multi-Agent Systems Architect |
| Prompt improvement | Engineering: Prompt Engineer |
| Analytics and reporting | Support: Analytics Reporter |
| Workflow design | Specialized: Workflow Architect |

**Search by relevance phase:**
For Phase 1 (design and validate), focus on High-relevance agents only. Medium-relevance agents are appropriate for Phase 2+. Low-relevance agents stay in library/ unless a specific need arises.

---

## 2. How to Evaluate

Before activating any agent, answer these four questions:

**1. Does it actually cover the task?**
Read the agent file. The "Primary purpose" and "Workflow Process" sections (if present) tell you whether it matches. Don't activate based on the name alone.

**2. What tools does it require?**
Check the `tools:` frontmatter field. If an agent requires Playwright, a specific API, or external service access, confirm that access exists before activating.

**3. How much of Ryan's time does activation require?**
Some agents need Ryan to provide a brief, review outputs, or configure inputs. If the agent requires more than 30 minutes of Ryan's time to activate, it should be queued, not immediately activated.

**4. Does it duplicate an existing agent?**
Check the Overlap Flags section in `AGENT_INDEX.md`. If a custom agent already covers the need, prefer the custom agent. If the library agent is better for a specific subtask, activate it with a clear scope boundary so both agents don't step on each other.

---

## 3. How to Customize

When a library agent covers the need but needs modification for AI Business Lab's context:

1. Copy the original file from `02-agents/library/agency-agents/` to `02-agents/custom/`.
2. Rename it to reflect the specific use: `marketing-seo-specialist.md` becomes `seo-specialist-contractor-niche.md`.
3. Modify the copy. Do not edit the original in `library/`. Keep the upstream version intact for reference.
4. In your customized version, add a header note:

```
> Customized from: 02-agents/library/agency-agents/[original-path]
> Changes: [brief description of what was changed and why]
```

**What to preserve from the original:**
- The core identity and role definition
- Critical rules and decision limits
- The deliverable templates (modify, not delete)

**What is safe to change:**
- Voice and tone to match Ryan's plain-language standards
- Industry focus (add "for contractors" context throughout)
- Tool requirements (add or remove based on actual availability)
- Output formats (simplify where the original is unnecessarily complex)

---

## 4. How to Activate

Activation means the agent is trusted to receive real tasks and produce outputs that influence decisions or client work.

**Activation checklist:**
- [ ] Agent file is in `02-agents/active/` (moved from library/ or custom/)
- [ ] `02-agents/active/ACTIVE_ROSTER.md` updated with: agent name, activation date, first assigned task, and scope boundary
- [ ] `AGENTS.md` (root) updated to reflect the new agent in the roster description
- [ ] `00-command-center/NEXT_ACTIONS.md` Agent Queue updated with the agent's first task
- [ ] Agent has been tested on one low-stakes task before receiving a client-facing task

**Moving a file to active:**
```bash
git mv 02-agents/library/agency-agents/[path]/[agent].md 02-agents/active/[agent].md
# or, if you customized it:
# the file is already in custom/ — no move needed; just update the roster
```

Custom agents in `02-agents/custom/` are always considered active. They do not need to be moved to `02-agents/active/`.

---

## 5. How to Retire

Retire an agent when:
- It has not been assigned a task in 30 days
- A newer or better agent covers the same need
- The business phase has moved past its relevance
- It produced consistently low-quality outputs that were not corrected through customization

**Retirement process:**
1. Move the file: `git mv 02-agents/active/[agent].md 02-agents/retired/[agent].md`
2. Add a one-line note at the top of the file explaining why it was retired and when.
3. Update `ACTIVE_ROSTER.md` — move the agent to the Retired section.
4. Update `AGENTS.md` if the agent was named there.
5. Update `NEXT_ACTIONS.md` if the agent had pending tasks — reassign or cancel them.

Do not delete retired agent files. They are reference material and can be reactivated.

---

## 6. Agent Communication Protocol

When assigning a task to a library or active agent, include context the agent cannot derive from its own definition:

```
Agent: [Agent Name]
Task: [Specific task]
Context: [What Ryan's business is, what phase we're in, what the output will be used for]
Inputs: [Exact files, data, or information the agent needs]
Output format: [Where the output should go — a file path, a section of NEXT_ACTIONS.md, etc.]
Needs Ryan: [Yes / No — and what specifically, if yes]
```

All agent outputs must be committed to the repo. No outputs live only in a conversation thread.
