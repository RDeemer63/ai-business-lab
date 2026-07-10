# Implementation Checklist

Run this before starting any build session. Run it again before committing.

---

## Before starting

- [ ] Read `00-command-center/NEXT_ACTIONS.md` -- what is the current task?
- [ ] Read `AGENTS.md` -- what are the current branch rules and agent rules?
- [ ] Check current branch -- am I on `agent/sandbox` or `agent/[feature]`? Never on `main`.
- [ ] Is this task operational (proceed) or structural (check if Chief Architect review is needed)?
- [ ] Are there open Needs Ryan items blocking this work?

## Structural change check

Is this session creating or modifying any of the following?
- A new directory in the repo root
- A file in `00-command-center/` (other than NEXT_ACTIONS.md or KNOWLEDGE_BASE.md)
- A file in `10-architecture/`
- A change to a frozen structure from `ARCHITECTURE_FREEZE_v1.md`

If yes: submit a review request to `11-review/pending/PR-N.md` first, unless Ryan has explicitly authorized the structural change in NEXT_ACTIONS.md.

If no: proceed.

## During the build

- [ ] Is the scope limited to what NEXT_ACTIONS.md specifies?
- [ ] Am I avoiding scope creep (no features Ryan did not ask for)?
- [ ] Am I creating new files only when no existing file can be updated?
- [ ] Am I committing in logical groups (one concern per commit)?
- [ ] Library agents: am I modifying anything in `02-agents/library/agency-agents/`? Stop. Never.

## Before committing

- [ ] Does each commit message describe what changed and why?
- [ ] Are all new files in the correct directory per the frozen structure?
- [ ] Is there any stale or half-finished content that should be cleaned up?
- [ ] Are there any external actions (emails, posts, spending) that need Ryan approval?

## Before closing the session

- [ ] Update `00-command-center/NEXT_ACTIONS.md` with the trail format from `AGENTS.md`
- [ ] Verify the branch is correct and all commits are pushed
- [ ] Is there a PR to open? If yes, target `main` (not a direct push)
- [ ] Are there any Needs Ryan items to add to NEXT_ACTIONS.md?

---

## Trail format reminder

```
### [Date] -- [Agent Name]

**What I did:**
**What changed:**
**What I recommend next:**
**Files touched:**
**Needs Ryan:**
```

Needs Ryan is the only section Ryan reads. Make it specific.
