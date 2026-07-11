# AGENTS.md — AI Business Lab

This file governs how AI agents work in this repository.

For full operating rules, see `00-command-center/OPERATING_PRINCIPLES.md`.
For the agent metadata database, see `02-agents/AGENT_REGISTRY.md`.
For the active roster, see `02-agents/active/ACTIVE_ROSTER.md`.

---

## Core principles

1. **Leave a trail.** Every agent session must end with an update to `00-command-center/NEXT_ACTIONS.md`.
2. **Branch discipline.** Work on `agent/sandbox` or `agent/[feature]`. Never push to `main` directly.
3. **Small PRs.** One concern per pull request.
4. **Decision records.** Non-obvious architectural or business decisions go in `08-decisions/` as dated markdown files.
5. **No gold-plating.** Build what the current phase needs. Defer everything else.
6. **Activate workflows, not agents.** Pull agents for a workflow. Return them to dormant when it ends.
7. **Library agents are never edited.** Customize in `02-agents/custom/` only.

---

## Current core team (Phase 1)

Three agents are permanently active. All others are dormant until a workflow requires them.

| Agent | File | Role |
|-------|------|------|
| Chief of Staff | `02-agents/custom/chief-of-staff.md` | Coordination, routing, command center |
| Project Manager | `02-agents/custom/project-manager.md` | Task tracking, queue health |
| Business Strategist | `02-agents/active/business-strategist.md` | Strategy analysis, opportunity evaluation |

### Permanent knowledge role

| Agent | File | Role |
|-------|------|------|
| Librarian | `02-agents/custom/librarian.md` | Institutional memory — records every experiment and decision |

### Supporting custom agents (always available)

| Agent | File | Role |
|-------|------|------|
| Business Research Agent | `02-agents/custom/business-research.md` | Idea scoring, market research |
| Newsletter Editor | `02-agents/custom/newsletter-editor.md` | Newsletter drafts, project documentation |

---

## Agent directory structure

```
02-agents/
  active/        — imported library agents approved for current use
  custom/        — agents built specifically for AI Business Lab
  library/       — full upstream library (276 files, read-only)
    agency-agents/   — msitarzewski/agency-agents (MIT)
    AGENT_INDEX.md   — full categorized index of library agents
    SELECTION_GUIDE.md — how to search, evaluate, and activate
  retired/       — agents removed from service
  AGENT_REGISTRY.md — queryable metadata for all evaluated agents
```

---

## Trail format

Every agent session must leave a note in `00-command-center/NEXT_ACTIONS.md`. This is a receipt, not just a log. It must include what was NOT done and why — so the next agent or human picking up the work knows exactly where to resume.

```
### [Date] — [Agent Name]

**Claimed:** [What task was taken on at the start of this session]
**Definition of Done:** [What completion looked like before starting — agreed up front]
**What I did:**
**What I did NOT do and why:** [Explicit. If nothing was skipped, say so.]
**Files touched:**
**Stop condition (if any):** [What blocked completion or required human input — empty if none]
**Needs Ryan:**
```

The **What I did NOT do and why** field is required even when nothing was skipped. Write "Nothing skipped — full scope completed." Agents that omit this field are leaving incomplete receipts.

---

## Communication flow

```
Ryan creates direction (NEXT_ACTIONS.md or issue)
    ↓
Chief of Staff routes to correct agent or workflow
    ↓
Agent(s) execute, commit outputs
    ↓
Pull Request opened (for significant changes)
    ↓
Ryan reviews Needs Ryan section only
    ↓
Merge
```

Ryan only touches the **Needs Ryan** section. Everything else runs without him.

---

## Idea Space rules

`01-business-ideas/IDEA_SPACE.md` is the studio's permanent idea archive.

- Agents tasked with finding, scoring, or researching ideas must NOT read it as a source or input
- Agents that surface any new idea during research MUST add it to IDEA_SPACE.md — even if it seems weak or off-topic
- Nothing gets removed from IDEA_SPACE.md — it is an append-only archive

---

## Tools agents may use

- Read/write files in this repo
- Create branches and PRs
- Update NEXT_ACTIONS.md and KNOWLEDGE_BASE.md
- Agents may NOT: send emails, post publicly, or spend money without Ryan's explicit approval in NEXT_ACTIONS.md
