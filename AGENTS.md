# AGENTS.md — AI Business Lab

This file governs how AI agents work in this repository.

---

## Core principles

1. **Leave a trail.** Every agent session must end with an update to `00-command-center/NEXT_ACTIONS.md` documenting what changed, what was decided, and what needs Ryan.
2. **Branch discipline.** Work on `agent/sandbox` or `agent/[feature]`. Never push to `main` directly.
3. **Small PRs.** One concern per pull request. Easier to review, easier to merge.
4. **Decision records.** Any non-obvious architectural or business decision goes in `08-decisions/` as a dated markdown file.
5. **No gold-plating.** Build what the current phase needs. Defer everything else.

---

## Agent roster (Phase 1)

### Chief of Staff
**File:** `02-agents/chief-of-staff.md`
**Scope:** Maintains NEXT_ACTIONS.md, routes tasks to the right specialist, surfaces blockers to Ryan, writes weekly status.

### Business Research Agent
**File:** `02-agents/business-research.md`
**Scope:** Scores business ideas, researches markets, analyzes competitors, estimates revenue paths.

### Newsletter Editor Agent
**File:** `02-agents/newsletter-editor.md`
**Scope:** Documents the experiment weekly. Drafts newsletter issues. Maintains the public-facing story of this project.

---

## Trail format

Every agent session must leave a note in `00-command-center/NEXT_ACTIONS.md` using this format:

```
## [Date] — [Agent Name]

**What I did:**
**What changed:**
**What I recommend next:**
**Files touched:**
**Needs Ryan:**
```

---

## Communication flow

```
Ryan creates direction (issue or NEXT_ACTIONS.md update)
    ↓
Claude Code drafts / builds / edits files
    ↓
Codex reviews / improves / challenges
    ↓
Pull Request opened
    ↓
Ryan reviews summary + decisions only
    ↓
Merge
```

Ryan only touches the **Needs Ryan** section. Everything else runs without him.

---

## Tools each agent may use

- Read/write files in this repo
- Create branches and PRs
- Update NEXT_ACTIONS.md and the decision log
- Agents may NOT: send emails, post publicly, or spend money without Ryan's explicit approval
