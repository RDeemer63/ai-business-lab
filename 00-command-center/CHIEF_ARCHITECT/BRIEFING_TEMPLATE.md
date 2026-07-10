# Chief Architect Briefing Template

Use this format for every CHATGPT_RECAP file. It lets the Chief Architect come into a new session already oriented — no context reconstruction needed.

---

## Current State

One paragraph. Where is the studio right now? What experiment, what gate, what's the open question?

## Decisions Required

Bullet list. What does the Chief Architect need to weigh in on this session? Be specific — vague questions produce vague answers.

## Evidence Since Last Review

What changed since the last briefing? Results, findings, surprises. Link to files.

| Item | What it showed | File |
|------|---------------|------|
| | | |

## Architectural Risk

One paragraph. If there is no current risk: "No architectural concerns." If there is a risk: name it, explain why it's acceptable now, and state when it stops being acceptable.

Example: "Current implementation introduces temporary coupling between GHL and the AI Conversation Engine. Acceptable until Gate 3 — at that point the capability must be extracted into its own service or the coupling becomes a production constraint."

## Questions for Chief Architect

Numbered. Specific. Each question should have a clear answer type (yes/no, recommendation, architectural judgment).

1.
2.
3.

## Recommended Reading Order

If the Chief Architect has 10 minutes before responding, what should they read first? Include estimated reading time per file.

1. File name (X min)
2. File name (X min)
3. File name (X min)

## Expected Output

What does the studio need from this review? A go/no-go? A recommendation? An architectural ruling? A new parking lot entry?
