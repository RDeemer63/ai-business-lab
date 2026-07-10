# Coding Standards

Standards for file quality and repo hygiene. These apply to all files created or modified by the Lead Engineer.

---

## Writing standards (all markdown files)

- No em dashes ever. Use a regular dash or rewrite the sentence.
- Plain, direct language. Short sentences. Active voice.
- No corporate words: leverage, synergy, holistic, robust, scalable.
- Bullet points for lists. Tables for comparisons. No walls of prose.
- Headers use sentence case (not Title Case for every word after the first).
- Every file has a clear purpose stated in the first paragraph or header.

## File naming

- All lowercase, words separated by underscores or hyphens (consistent within a directory)
- Descriptive, not clever: `EXPERIMENT_ZERO.md` not `E0.md`
- Dates in filenames use ISO format: `2026-07-09`
- PR files use sequential numbers: `PR-1.md`, `PR-2.md`

## Directory structure rules

- New directories require a README.md or .gitkeep
- Empty directories exist only when they are holding a place for a documented future use
- If a directory has been empty for 30 days with no documented purpose, evaluate removing it
- Do not nest directories more than three levels deep unless there is a specific reason

## Agent definition files

- Every agent definition file starts with a clear role statement
- Source library agents are always credited in a comment at the top of custom agents
- Custom agents follow the format: role statement, capabilities, constraints, output format
- No agent definition should require Ryan to re-explain context on every session

## Commit message format

```
[Type]: [Short description]

[Optional: one paragraph explaining why, not what]
```

Types: `feat` (new capability), `fix` (corrects a mistake), `docs` (documentation only), `refactor` (restructures without changing behavior), `chore` (maintenance)

Examples:
- `feat: Add business research agent with 12-point scoring rubric`
- `docs: Architecture Freeze v1.0 -- ADRs, role directories, review structure`
- `chore: Clean up stale .gitkeep files from retired experiment directories`

## What counts as a good commit

- One logical concern per commit
- The repo is in a working state after the commit
- The commit message describes what changed without requiring context
- No credentials, API keys, or personal information in committed files
- No half-finished work (if something is in progress, finish it or stash it)

## Branch discipline

- Work happens on `agent/sandbox` or `agent/[feature]`
- Never push directly to `main`
- PRs target `main`
- Branch names are lowercase with dashes: `agent/experiment-zero`, `agent/workflow-validate`
