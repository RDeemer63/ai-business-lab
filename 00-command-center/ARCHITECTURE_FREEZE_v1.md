# Architecture Freeze v1.0

**Date:** 2026-07-09
**Status:** Active
**Frozen by:** Ryan Deemer (Founder), Chief Architect (ChatGPT), Lead Engineer (Claude Code)

This document freezes the organizational architecture of AI Business Lab. The structures below may not change without evidence from experiments or an explicit ADR process.

---

## The Three Laws

These laws govern how the studio operates. They are not guidelines. They cannot be overridden by convenience, excitement, or a good idea.

### Law 1: The repository is the source of organizational state.

If it is not in the repo, it did not happen. New sessions reconstruct context from committed files, not conversation history. The organization does not rely on any AI model's in-context memory.

### Law 2: Architecture changes by evidence, not ideas.

A new structural idea goes in PARKING_LOT.md. It earns its way into the architecture by demonstrating a real problem that the current structure cannot solve. The evidence standard: "which experiment revealed this need?" If you cannot answer that question, the idea is not ready.

### Law 3: Intelligence is replaceable. Organizational state is not.

Claude Code, ChatGPT, and any future AI models are the current implementation of their roles. They will be upgraded, replaced, and deprecated. The role directories survive. The ADRs survive. The lessons survive. The intelligence is a means, not the end.

---

## Architecture Budget

**Maximum:** 1 architecture sprint per month.
**Minimum:** 3 operating sprints between architecture sprints.

An architecture sprint is any session whose primary output is structural changes to the organization -- new directories, new roles, new governance documents. Operating sprints build businesses.

The Architecture Budget exists because architecture work is easy to mistake for progress. The studio succeeds by launching businesses, not by perfecting its own structure.

---

## Frozen Structures

The following structures are frozen as of v1.0. They may not be changed without an ADR.

### Repository organization

```
00-command-center/    -- command center: actions, principles, knowledge, role directories
01-business-ideas/    -- idea pipeline and evaluation
02-agents/            -- agent definitions and library
03-workflows/         -- reusable workflow documentation
04-experiments/       -- active and completed experiments
09-lessons/           -- institutional memory: decisions, post-mortems, pattern reports
10-architecture/      -- ADRs and architecture records
11-review/            -- cross-model review workflow (pending/ and completed/)
```

Numbers are intentional. New directories must fit the existing numbering logic or require an ADR.

### Core governance

- Three Laws (above) -- cannot be modified, only superseded by a v2 freeze
- Architecture Budget -- 1 sprint/month, 3 operating sprints minimum between
- Evidence standard for architecture changes: name the experiment that revealed the need
- PARKING_LOT.md holds ideas that have not earned their way in

### Role model

Three permanent roles, each with a directory in `00-command-center/`:

| Role | Current model | Directory |
|------|--------------|-----------|
| Chief Architect | ChatGPT | `00-command-center/CHIEF_ARCHITECT/` |
| Lead Engineer | Claude Code | `00-command-center/LEAD_ENGINEER/` |
| Founder | Ryan Deemer | `00-command-center/FOUNDER/` |

Roles belong to the organization. Models are the current implementation.

### Agent governance

- Core team maximum: 3 permanently active agents (Phase 1)
- Workflow-first activation: agents are dormant until a workflow requires them
- Library agents (02-agents/library/) are never edited
- Agent metadata tracked in AGENT_REGISTRY.md

### Review workflow

Cross-model reviews (Claude Code requests a Chief Architect review):
1. Lead Engineer creates `11-review/pending/PR-N.md`
2. Chief Architect reads it, creates `11-review/completed/PR-N-review.md`
3. Lead Engineer reads response and acts on it

Reviews are committed artifacts. They are not lost in conversation threads.

### Control loop

```
State (repo) --> Intelligence reads State --> Execution changes State --> New State
```

There is no hierarchy above this loop. The repo is the API. Intelligence reads it and writes to it. Ryan's role is to define direction and approve at human gates -- not to relay messages between agents.

---

## What Is Not Frozen

The following may change as the studio learns:

- Which specific agent files are active
- Individual workflow steps and sequences
- Business ideas under evaluation
- Content of knowledge base entries
- Specific implementation details in role directories

---

## How to Change a Frozen Structure

1. Identify which experiment demonstrated that the current structure is causing a real problem
2. Write an ADR in `10-architecture/` describing the context, decision, and consequences
3. Get Ryan's approval on the ADR
4. Implement the change
5. Update this document if the change affects a frozen structure

You may not change a frozen structure because you have a good idea, because the current structure feels limiting, or because a different approach seems elegant. You may only change it because evidence shows the current structure is causing measurable harm to the studio's operating velocity.

---

## What Lives in PARKING_LOT.md

Ideas that have not earned their way into the architecture wait in PARKING_LOT.md. A parked idea has:
- A clear description of what it proposes
- The problem it claims to solve
- The evidence it needs before it can be considered
- A date when it was parked

Parking an idea is not rejection. It is an honest acknowledgment that the idea has not been tested yet.

---

## Freeze History

| Version | Date | Summary |
|---------|------|---------|
| 1.0 | 2026-07-09 | Initial architecture freeze. Three Laws, Architecture Budget, role model, control loop, review workflow. |
