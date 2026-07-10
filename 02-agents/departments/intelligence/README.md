# Intelligence Department

**Mission:** Make the studio smarter over time.

**Status:** Permanent — never goes dormant.

## Why this department exists

Without Intelligence, the studio gets bigger but never gets better. This department is the organizational immune memory. It ensures every experiment teaches something, every failure is documented, every repeated mistake gets noticed, and every agent definition that produces bad outputs gets fixed.

## Agents

| Agent | File | Role |
|-------|------|------|
| Librarian | `custom/librarian.md` | Maintains KNOWLEDGE_BASE.md; records experiment results |
| Historian | `custom/historian.md` | Records decisions with full context; writes post-mortems |
| Pattern Analyst | `custom/pattern-analyst.md` | Monthly: surfaces what's working and what keeps failing |
| Knowledge Curator | `custom/knowledge-curator.md` | Updates agent definitions based on Pattern Analyst findings |

All four agents are permanently active. They do not go dormant between workflows.

## Output directory

`09-lessons/` and `00-command-center/KNOWLEDGE_BASE.md`

## Cadence

- Librarian: after every experiment completes
- Historian: after every merged PR with strategic implications; after every business kill
- Pattern Analyst: first day of each month
- Knowledge Curator: within 5 days of each Pattern Analyst report
