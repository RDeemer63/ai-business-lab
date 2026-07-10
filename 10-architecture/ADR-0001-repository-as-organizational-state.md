# ADR-0001: Repository as Organizational State

**Date:** 2026-07-09
**Status:** Accepted
**Deciders:** Ryan Deemer (Founder), Chief Architect (ChatGPT), Lead Engineer (Claude Code)

---

## Context

AI Business Lab is an autonomous venture studio where multiple AI models (Claude Code, ChatGPT, future models) and a human founder (Ryan) collaborate on business creation. We needed a way for the organization to function coherently when:

- Different AI models have no persistent memory between sessions
- Ryan cannot serve as the communication hub between AI agents
- The organization must survive replacing any AI model with a different model or version
- Multiple agents may work on the same project at different times without losing context

The question was: where does organizational knowledge live?

---

## Decision

**The GitHub repository is the source of organizational state.**

This means:

1. If something happened and it is not in the repository, it did not happen.
2. A new AI session can reconstruct full context by reading the repository.
3. All decisions, experiments, workflows, and institutional knowledge are committed files.
4. The repository is not storage. It is the organization.

---

## Consequences

**What this enables:**

- Any AI model can pick up where any other left off without Ryan serving as translator
- Organizational knowledge survives model deprecation, API outages, and session limits
- The organization improves over time because every lesson is a committed file
- Decisions have a clear audit trail -- who decided, when, and why

**What this requires:**

- Every agent session must commit its outputs before ending
- No knowledge may live only in a conversation thread
- The Librarian role exists specifically to enforce this -- recording experiments and decisions that would otherwise be lost
- NEXT_ACTIONS.md is updated at the end of every session, no exceptions

**What this rules out:**

- Relying on an AI model's in-context memory across sessions
- Keeping institutional knowledge in email threads, Slack messages, or mental notes
- Declaring work "done" without committing the result

---

## Evidence

This decision was made before the studio had operational evidence. It is based on the structural requirement that AI models have no persistent memory and Ryan cannot function as the memory layer for an autonomous studio.

**Review trigger:** If we find that the repository-as-state model creates more friction than it prevents, open an ADR to revise it. Trigger: two consecutive operating sprints where agents spent more time maintaining state than executing work.

---

## Related decisions

- ADR-0002: Roles Defined by Documents, Not Models
