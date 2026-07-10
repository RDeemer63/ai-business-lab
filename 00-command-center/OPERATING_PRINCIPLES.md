# Operating Principles

**Version:** 1.1
**Date:** 2026-07-10
**Status:** Active

These principles govern how AI Business Lab operates. They exist to prevent drift, duplication, and the gradual accumulation of complexity that kills small systems. Every agent, every workflow, and every decision should be consistent with these principles.

---

## Constitutional Rule: How Principles Are Added

**No operating principle may be added unless it can be traced to a specific experiment, decision, or post-mortem.**

Every principle must cite its origin — the experiment that produced the evidence, the decision that exposed the gap, or the post-mortem that documented the failure. Principles derived from inspiration or good intentions alone are not admitted. This document accumulates principles the same way science accumulates theories: from repeated observation, not from philosophy.

When adding a new principle, include:
- The principle itself
- The source (experiment number, decision ID, or post-mortem reference)

*This rule was itself sourced from the evidence of Principle 12 — the first principle this organization earned rather than invented.*

---

## Core Principles

### 1. Humans approve. AI executes.

No agent takes an action that affects the outside world — sending a message, publishing content, spending money, contacting a person — without Ryan's explicit approval. Internal work (research, drafting, analysis, file creation) runs autonomously. External actions require a Needs Ryan entry in NEXT_ACTIONS.md first.

### 2. No duplicate agents.

Before creating or activating a new agent, search the library. If a library agent covers the need at 80% or better, use it. If customization is needed, fork the library agent into `custom/` — do not create a parallel agent that does the same job under a different name. Check AGENT_REGISTRY.md before every activation request.

### 3. No duplicate knowledge.

If information exists in one file, do not copy it to another file — reference it. NEXT_ACTIONS.md is the source of truth for current task state. AGENT_REGISTRY.md is the source of truth for agent metadata. The activity log is the record of what happened. If something needs to live in two places, one of the two places is wrong.

### 4. Every experiment is measured.

A validation test that produces no documented result did not happen. Every test in NEXT_ACTIONS.md must have a defined success metric before it starts and a documented result when it ends. The Librarian records all results. Results inform future decisions — they do not disappear into conversation threads.

### 5. Every failure is documented.

A failed experiment is more valuable than an undocumented success. When something does not work, the Librarian records what was tried, what the result was, and what was learned. The goal is to fail fast and not repeat the same failure twice.

### 6. Every workflow is reusable.

If a sequence of agent tasks is performed more than once, it becomes a documented workflow in `03-workflows/`. Workflows define the agents involved, the sequence, the inputs, the outputs, and the success criteria. Workflows are the product of institutional learning.

### 7. Everything is version controlled.

No knowledge lives only in a conversation thread. No decision lives only in someone's memory. If it happened, it is committed to the repository. This is the rule that makes the system durable.

### 8. Library agents are never edited.

Files in `02-agents/library/agency-agents/` are upstream files. They are never modified. If a library agent needs customization, copy it to `02-agents/custom/`, add a header noting the source, and modify the copy. This keeps upstream files clean for future syncing.

### 9. Custom agents inherit context from library agents.

When creating a custom agent, start from the most relevant library agent as a base. Add context specific to AI Business Lab (contractor market, Ryan's voice, current phase) rather than building from scratch. Reference the source file in the custom agent header.

### 10. Activate workflows, not agents.

Agents do not have permanent jobs. Workflows require agents temporarily. The Chief of Staff maintains a small permanent core team (3 agents maximum in Phase 1) and assembles larger teams only for defined workflows. When a workflow ends, the team shrinks back to the core. Agent sprawl is a failure mode.

### 11. The machine improves itself.

Every six months, the Chief of Staff and Librarian conduct an audit: which agents were used, which weren't, what workflows ran, what institutional knowledge was captured. The goal is that Business #12 is launched faster and with fewer mistakes than Business #1 because the machine learned from each prior attempt.

### 12. Do not answer tomorrow's portfolio question with today's experiment.

Experiments validate value. Portfolio decisions — standalone product, Tulboxx feature, Throttled Up capability, or something else — happen after the value is confirmed. Building the wrong container before the market proves the value is premature. Run the experiment. Get the evidence. Then decide where it lives.

*Source: Experiment 001 design. The Tulboxx integration question was deliberately deferred until after Gate 3. That discipline is now permanent.*

### 13. Build infrastructure only after a workflow has demonstrated repeatable value.

Validated customer demand is necessary but not sufficient. A workflow must be run manually enough times to prove it is repeatable before it earns automation. Automating a workflow that has only run once optimizes something you do not yet understand. Run it manually first. When the manual version is producing consistent results and the bottleneck is clearly the execution speed — not the process design — then build the infrastructure.

*Source: Experiment 001 build session. The Claude-powered webhook server (AI Conversation Engine) was identified as a better architecture than GHL's native AI, but parked until Gate 3 passes and a paying client makes setup speed a real constraint. That decision has been made twice now — once for the webhook server, once for the Prospect Factory. The pattern is permanent.*

---

## Current Phase Rules (Phase 1)

- Core team maximum: 3 agents
- No client-facing work until offer is defined and Ryan approves
- No external communications without explicit Needs Ryan approval
- All research outputs committed to `01-business-ideas/` before Ryan makes any decision
- Validation tests run before any build decision is made

---

## What These Principles Protect Against

**Agent sprawl:** Activating 15 agents because they might be useful creates coordination overhead that exceeds their value. The activation limit and workflow model prevent this.

**Knowledge rot:** Information that lives in conversation threads instead of the repo becomes inaccessible. The version control and Librarian principles prevent this.

**Founder dependency creep:** Building systems that require Ryan's personal involvement to function defeats the purpose. The "humans approve, AI executes" split keeps Ryan at the approval level, not the execution level.

**Groundhog day:** Running the same experiment twice because the first result wasn't documented. The measurement and failure documentation principles prevent this.
