# Review Workflow

This directory is how the Lead Engineer and Chief Architect communicate without Ryan serving as a message bus.

Reviews are committed artifacts. They are searchable, referenceable, and permanent. They do not live in conversation threads.

---

## When a review is needed

A Chief Architect review is required before:

- Adding a new directory to the repository root
- Adding a new permanent role to the organization
- Changing a frozen structure from `00-command-center/ARCHITECTURE_FREEZE_v1.md`
- Adding or modifying an ADR in `10-architecture/`
- Updating the Architecture Budget or evidence standard
- Proposing a new governance layer

It is NOT required for:

- Agent definitions and activations
- Workflow documentation updates
- Business idea research and evaluation
- Experiment design (unless proposing a structural change)
- Knowledge base entries

When in doubt: if the change touches `00-command-center/` or `10-architecture/`, request a review. If it touches `01-`, `02-`, `03-`, `04-`, or `09-`, proceed without review.

---

## How it works

**Step 1: Lead Engineer creates the request**

Create a file in `pending/`:

```
11-review/pending/PR-1.md
```

Use sequential numbers. Include:
- What is being proposed
- What problem it solves
- What evidence supports the need
- What alternatives were considered
- The specific question you want the Chief Architect to answer

Commit the file and notify Ryan.

**Step 2: Ryan shares with Chief Architect**

Ryan copies or shares the PR file with ChatGPT (Chief Architect). The Chief Architect reads it along with the files in `00-command-center/CHIEF_ARCHITECT/`.

**Step 3: Chief Architect responds**

The Chief Architect produces a response. Ryan commits it to:

```
11-review/completed/PR-1-review.md
```

**Step 4: Lead Engineer acts**

The Lead Engineer reads the completed review and acts on the verdict (Approve / Reject / Park / Revise).

---

## Directory structure

```
11-review/
  pending/        -- review requests awaiting Chief Architect response
  completed/      -- completed reviews (permanent record)
  architecture/   -- placeholder for future architecture-specific review type
  business/       -- placeholder for future business-specific review type
  engineering/    -- placeholder for future engineering-specific review type
```

The `architecture/`, `business/`, and `engineering/` subdirectories are placeholders. They hold space for more specialized review types as the studio matures. They are not used in Phase 1.

---

## Review response format

See `00-command-center/CHIEF_ARCHITECT/REVIEW_PROCESS.md` for the full format.

Verdict options: Approve / Reject / Park / Revise.

---

## Review numbering

Reviews are numbered sequentially: PR-1, PR-2, PR-3.

"PR" stands for "pending review," not "pull request" (though structural changes often result in a git PR). The same number is used for both the request file and the response file (with `-review` appended to the response).

---

## This directory in future phases

In Phase 2 and beyond, this review workflow may be partially automated. The pending/ directory structure is designed to support automation: a script could watch for new files, trigger a notification, and route them appropriately. That automation is parked until Phase 1 is operating smoothly.
