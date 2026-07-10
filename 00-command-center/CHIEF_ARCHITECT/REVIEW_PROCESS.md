# Review Process

How the Chief Architect receives work, reviews it, and returns findings.

---

## When a review is needed

A Chief Architect review is required before:

- Adding a new directory to the repository root
- Adding a new permanent role to the organization
- Changing a frozen structure from ARCHITECTURE_FREEZE_v1.md
- Adding or modifying an ADR
- Updating the Architecture Budget or evidence standard
- Proposing a new governance layer (new review type, new approval gate, new audit cadence)

A Chief Architect review is NOT required for:

- Agent definitions and activations
- Workflow documentation updates
- Business idea research and evaluation
- Experiment design (unless the experiment itself proposes a structural change)
- Knowledge base entries
- NEXT_ACTIONS.md updates

When in doubt: if the change affects a file in `00-command-center/` or `10-architecture/`, request a review. If the change affects operational files (`01-`, `02-`, `03-`, `04-`, `09-`), proceed without review.

---

## How to request a review

The Lead Engineer creates a review request file in `11-review/pending/`:

```
11-review/pending/PR-N.md
```

Where N is the next sequential number.

The file contains:
- What is being proposed
- What problem it solves
- What evidence supports the need
- What alternatives were considered
- What specific question the Lead Engineer wants the Chief Architect to answer

The Lead Engineer commits the file and notifies Ryan. Ryan shares it with ChatGPT (Chief Architect).

---

## How to conduct a review

The Chief Architect reads the review request. Then reads:
- `DESIGN_PHILOSOPHY.md` (is this consistent with core beliefs?)
- `QUESTIONS_I_ALWAYS_ASK.md` (run through the checklist)
- `COMMON_FAILURE_PATTERNS.md` (does this match a known failure mode?)
- `../../10-architecture/` (does this contradict any existing ADR?)

The Chief Architect produces a review response and Ryan commits it to:

```
11-review/completed/PR-N-review.md
```

---

## Review response format

```markdown
# Review: [Title from PR-N.md]

**Request:** PR-N
**Reviewed:** [Date]
**Verdict:** Approve / Reject / Park / Revise

## Verdict rationale

[2-4 sentences explaining the verdict]

## Checklist

- Problem clearly stated: Yes / No
- Evidence sufficient: Yes / No
- Simplest solution: Yes / No
- Architecture Budget respected: Yes / No
- Maintenance cost acceptable: Yes / No

## Specific concerns

[Any items the Lead Engineer should address before proceeding]

## What I'd change

[Specific suggestions if verdict is Revise]

## What goes to PARKING_LOT.md

[Any adjacent ideas from this review that should be parked]
```

---

## Verdicts

**Approve:** The Lead Engineer may proceed with the proposed change.

**Reject:** The change is not appropriate for the architecture. The review explains why. The Lead Engineer does not proceed. The idea may be parked for future consideration.

**Park:** The change has merit but lacks evidence. The Lead Engineer creates an entry in PARKING_LOT.md with the evidence needed to graduate it.

**Revise:** The change is on the right track but needs modification. The review specifies what to change. The Lead Engineer submits a revised PR-N-rev.md.

---

## Response timeline

There is no automated response. The Chief Architect is human-triggered and Ryan-mediated. Reviews are not blocking for operational work. While a review is pending, the studio continues running experiments and validating ideas. Reviews are blocking only for the specific structural change under review.

---

## Review as institutional memory

Every completed review is a committed artifact. When future sessions need to understand why a structural decision was made, the review trail provides that context. Reviews are not overhead. They are the record of how the architecture evolved.
