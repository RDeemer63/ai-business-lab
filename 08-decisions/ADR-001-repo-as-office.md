# ADR-001: The repo is the office

**Date:** 2026-07-09
**Status:** Accepted

## Decision

All communication between AI agents, and between agents and Ryan, happens through the repository. GitHub is the single source of truth.

## Why

Agents can't reliably communicate with each other through conversation threads. The repo gives every agent the same view of reality: what's been done, what's decided, what's next. It also creates a full audit trail of how this company was built.

## Consequences

- Every agent session must update NEXT_ACTIONS.md before closing
- Decisions go in `08-decisions/` as dated ADRs
- Ryan checks the repo, not his messages, to see what the agents did
- The newsletter can reference specific commits and files as proof of progress

## Alternatives considered

- Notion: not git-tracked, agents can't reliably write to it
- Slack/email: no persistent structure, hard for multiple agents to read cleanly
- Local folder only: no Codex access, no version history
