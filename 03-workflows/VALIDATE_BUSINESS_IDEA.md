# Workflow: Validate a Business Idea

**Status:** READY
**Version:** 1.0
**Created:** 2026-07-09

---

## Goal

Produce a 7-day validation signal for one business idea without building anything.

---

## Trigger

Ryan selects a finalist idea from `01-business-ideas/COMBINED_COMPARISON.md`.

---

## Agents required (temporary activation)

| Agent | Status | Role in workflow |
|-------|--------|----------------|
| Chief of Staff | permanent | Routes tasks, updates NEXT_ACTIONS.md |
| Business Strategist | permanent | Designs the validation test |
| Trend Researcher | dormant — activate | Researches target customer and channel |
| Outbound Strategist | dormant — activate | Designs outreach sequence |

Trend Researcher and Outbound Strategist return to dormant after Step 3.

---

## Sequence

### Step 1 — Business Strategist: Define the test

- **Input:** Idea profile from `IDEA_PIPELINE.md` or `CLEAN_SLATE_PIPELINE.md`
- **Task:** Write a one-page validation plan — target customer, hook, channel, success metric, 7-day timeline
- **Output:** `04-experiments/[idea-slug]/VALIDATION_PLAN.md`
- **Definition of Done:** VALIDATION_PLAN.md exists, contains a specific measurable signal ("3 genuine interest expressions in 7 days"), and Ryan has approved it
- **Stop condition:** If the idea cannot be tested without building something first, flag it — do not invent a workaround. Move to "Needs Ryan."
- **Ryan touchpoint:** Approve the plan before Step 2 begins

---

### Step 2 — Trend Researcher: Find the customers

- **Input:** Approved validation plan from Step 1
- **Task:** Identify 25-50 specific prospects (communities, contacts, channels) where the target customer is reachable
- **Output:** `04-experiments/[idea-slug]/PROSPECT_LIST.md`
- **Definition of Done:** PROSPECT_LIST.md contains at least 25 specific, reachable prospects with channel noted for each
- **Stop condition:** If fewer than 25 reachable prospects can be identified, record what was found and flag — do not pad with low-quality contacts. Move to "Needs Ryan."
- **Ryan touchpoint:** None — research only, no external contact

---

### Step 3 — Outbound Strategist: Write the hook

- **Input:** Prospect list, validation plan
- **Task:** Write the outreach message, subject line, and follow-up sequence
- **Output:** `04-experiments/[idea-slug]/OUTREACH_DRAFT.md`
- **Definition of Done:** OUTREACH_DRAFT.md contains one primary message, one subject line variant, and one follow-up. All three are reviewed and ready for Ryan's approval.
- **Stop condition:** If the message requires claiming something the studio cannot deliver, flag it — do not write misleading copy. Move to "Needs Ryan."
- **Ryan touchpoint:** Approve all messages before Ryan sends any of them

---

### Step 4 — Ryan: Run the test

- Ryan sends the outreach or posts in communities
- Timeline: 7 days
- No agent involvement during this step
- Ryan notes all responses in `04-experiments/[idea-slug]/RAW_RESPONSES.md` (or just tells the Chief of Staff at the end)
- **Definition of Done:** 7 days have elapsed AND Ryan has reported responses (even if zero)

---

### Step 5 — Chief of Staff: Record the result

- **Input:** Ryan's report on responses, interest level, conversion
- **Task:** Write `04-experiments/[idea-slug]/RESULT.md` with the result, the metric, and a go/no-go recommendation
- **Librarian task:** Record in `00-command-center/KNOWLEDGE_BASE.md`
- **Output:** Go / No-go recommendation in NEXT_ACTIONS.md
- **Definition of Done:** RESULT.md exists, KNOWLEDGE_BASE.md is updated, and a clear go/no-go recommendation is written in NEXT_ACTIONS.md with evidence cited
- **Stop condition:** If responses are ambiguous (polite interest but no buying signal), say so explicitly — do not interpret ambiguity as a go. Call it inconclusive and recommend a second iteration.

---

## Success criteria

- At least 3 genuine expressions of interest (not polite replies)
- At least 1 prospect willing to pay before the product exists

## Failure criteria

- Zero responses after 7 days with a cleaned-up message
- Responses only from people who would not pay

---

## Outputs

```
04-experiments/[idea-slug]/
  VALIDATION_PLAN.md
  PROSPECT_LIST.md
  OUTREACH_DRAFT.md
  RAW_RESPONSES.md
  RESULT.md
```

Plus one entry in `00-command-center/KNOWLEDGE_BASE.md`.

---

## Experiment folder naming

Use a short, lowercase, hyphenated slug based on the idea name:

- `ai-content-subscription`
- `ada-compliance-monitoring`
- `lead-followup-service`
