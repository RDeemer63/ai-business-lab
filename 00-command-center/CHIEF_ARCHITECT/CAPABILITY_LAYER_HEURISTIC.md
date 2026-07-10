# Capability Layer Heuristic

Before any capability discussion, answer three questions in order. Do not jump to implementation until all three are answered.

---

## The Three Questions

### 1. Is this knowledge?

Knowledge is a specification, a recipe, a definition, or a classification. It lives in a document. It costs nothing to create and nothing to run. It does not require code or tools.

Examples: Prospect Recipe, Principle, ICP definition, scoring rubric, interview guide.

**If the answer is yes:** Write it down. It belongs in the repo. No build required.

---

### 2. Is this a workflow?

A workflow is a repeatable sequence of steps that can be executed using existing tools, people, or agents — without writing new software. It may use Clay, Apollo, GHL, Claude, spreadsheets, or a checklist. The steps are defined. The tools already exist.

Examples: Prospect Factory (Clay + enrichment + scoring), Gate 2 interview process, post-mortem ritual, experiment close-out sequence.

**If the answer is yes:** Document the workflow. Run it manually at least twice before automating any part of it. The workflow earns automation only after it has demonstrated repeatable value.

---

### 3. Is this software?

Software is custom-built code that automates or replaces part of a workflow because the workflow has proven repeatable and the bottleneck is now execution speed. Software is never the first answer.

Examples: AI Conversation Engine (webhook server), Prospect Intelligence Engine, Studio Health Dashboard.

**If the answer is yes:** Apply the Commodity/Build filter first — can you buy 80% of this today? If yes, buy it. Build only the differentiating 20%.

---

## The Commodity / Build Filter

Before building any software, ask:

| Question | If YES |
|----------|--------|
| Can we buy 80% of this today? | Buy it. Invest saved time in the differentiating 20%. |
| Does it encode knowledge that is unique to this organization? | Build it. This is intellectual property. |
| Does it improve every future experiment? | Consider internal platform status — but only after 3+ experiments have needed it. |
| Does it become permanent organizational knowledge? | Preserve it regardless of whether the tool survives. |

**Commodity:** Email delivery, prospect enrichment, CRM, scheduling, payments.
**Competitive advantage:** Lead scoring rules based on our data, conversation logic tuned to our market, pattern analysis across our experiments, venture governance, organizational memory.

---

## Common Mistakes This Heuristic Prevents

**Treating a workflow as software.** The Prospect Factory is orchestration — Clay + a documented sequence. It is not a software project until the workflow runs at a scale where manual execution is the bottleneck.

**Treating knowledge as a workflow.** A Prospect Recipe is a document. Writing it down does not require running a tool. Writing it requires having the evidence.

**Building software before running the workflow.** You cannot automate what you do not yet understand. Manual execution teaches you what the automation actually needs to do.

---

*Source: Experiment 001 design session. The Prospect Factory discussion surfaced the mistake of conflating workflow with software. Principle 13 was sourced from the same session.*
