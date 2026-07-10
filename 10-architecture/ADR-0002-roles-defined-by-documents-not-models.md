# ADR-0002: Roles Defined by Documents, Not Models

**Date:** 2026-07-09
**Status:** Accepted
**Deciders:** Ryan Deemer (Founder), Chief Architect (ChatGPT), Lead Engineer (Claude Code)

---

## Context

AI Business Lab uses two primary AI models in distinct roles: Claude Code (Lead Engineer) and ChatGPT (Chief Architect). A natural question arose: what happens when these models are deprecated, upgraded, or replaced? If the roles live in the models, the organization loses institutional memory every time a model changes.

A second problem: new sessions of the same model also start with zero context. Claude Sonnet 4.6 today does not remember what Claude Sonnet 4.6 did last week. Without role documents, every new session starts from scratch.

---

## Decision

**Roles belong to the organization. AI models are the current implementation.**

Each role has a directory in `00-command-center/`:

- `CHIEF_ARCHITECT/` -- accumulated design judgment for whoever fills the architect role
- `LEAD_ENGINEER/` -- implementation standards for whoever fills the engineering role
- `FOUNDER/` -- investment criteria and decision rules for Ryan

When a new AI session begins, the first action is to read the role directory. The session inherits the role's accumulated judgment, philosophy, and standards -- not just instructions, but the reasoning behind them.

**The role outlasts the model.**

---

## Consequences

**What this enables:**

- Model transitions do not require rebuilding institutional knowledge from scratch
- A new version of Claude Code reads LEAD_ENGINEER/ and knows what standards apply
- A new version of ChatGPT reads CHIEF_ARCHITECT/ and knows what patterns to look for
- Ryan can hand off the Founder role (to a partner, investor, or future co-founder) because the criteria are documented
- The organization grows smarter with each session rather than resetting

**What this requires:**

- Role directories must be updated when standards change -- not just followed
- When a model makes a non-obvious judgment call, the reasoning goes in the role directory
- COMMON_FAILURE_PATTERNS.md in each role directory must be updated when a failure occurs
- Role documents are part of every commit that changes a role-level standard

**What this rules out:**

- Keeping engineering standards only in the Lead Engineer's mental model
- Keeping architectural principles only in ChatGPT's conversation history
- Treating "I remember from last time" as a reliable substitute for committed documentation

---

## Role directory structure

Each role directory contains:

| File | Purpose |
|------|---------|
| `README.md` | Who this role is, what it does, how to onboard a new instance |
| `[ROLE]_PHILOSOPHY.md` | Core beliefs that drive decisions -- the "why" layer |
| `QUESTIONS_I_ALWAYS_ASK.md` or `IMPLEMENTATION_CHECKLIST.md` | The repeatable process for role-specific work |
| `REVIEW_PROCESS.md` or `CODING_STANDARDS.md` | Standards for evaluating work quality |
| `COMMON_FAILURE_PATTERNS.md` or `DECISIONS_NOT_TO_BUILD.md` | What this role has learned to watch out for |

---

## Evidence

This decision was made before the studio had operational evidence. It is based on the structural reality that AI models have no persistent memory and the need for the organization to accumulate judgment over time.

**Review trigger:** If we find that role documents are not being read in practice (agents produce work inconsistent with role standards), open an ADR to revise the onboarding process. Trigger: two operating sprints where an agent's output contradicted its role standards.

---

## Related decisions

- ADR-0001: Repository as Organizational State
