# Risk Tolerance

What risks this studio accepts, what risks it does not, and how to think about risk at the portfolio level.

---

## What this studio is optimized for

Speed of learning, not certainty of outcome. The studio accepts a high rate of idea failure because the kill criteria and validation cycle are designed to fail fast and cheap. A failed experiment that costs one week is acceptable. A failed business that costs six months of Ryan's time is not.

This is a high-variance, low-downside model. Many small bets. Fast feedback. Hard kills on clear criteria.

---

## Acceptable risks

**High idea failure rate**
Most ideas will fail validation. This is expected. The studio is designed to absorb it. A 20-30% go rate on validated ideas would be a strong result. Anything above that likely means the kill criteria are not being applied rigorously enough.

**Building before there is a market**
Validation tests are designed to test market demand before building anything. But the test itself has a cost. Spending one week on a validation test for an idea that turns out to have no market is acceptable. The cost is bounded.

**Agent quality variance**
AI agent output will be inconsistent. Research quality will vary. Analysis will have gaps. This is managed by the Librarian (recording lessons from every output) and by the review process. It is not a risk that can be eliminated, only managed.

**Opportunity cost**
Pursuing one idea means not pursuing another during the same sprint. This is an accepted structural risk of a single-portfolio-at-a-time model in Phase 1.

---

## Unacceptable risks

**Ryan's time beyond the threshold**
Any business model that requires more than 20 hours of Ryan's time to stabilize is killed under the kill criteria. This is a non-negotiable boundary. The studio model depends on Ryan's time being available for the next idea.

**External commitments before validation**
No money is spent, no clients are signed, no communications are sent externally before a validation test produces a go signal. External commitments lock the studio into an idea before evidence justifies the lock-in.

**Reputation risk**
Ryan's personal and professional reputation is a studio asset. Nothing is done under Ryan's name without Ryan's explicit approval. No agent represents Ryan externally. No public-facing content is published without review.

**Irreversible architectural decisions without evidence**
Changing the frozen architecture without evidence and an ADR is a risk to the studio's long-term coherence. The architecture represents accumulated judgment. Overriding it without process undermines the foundation.

**Debt accumulation**
Building technical debt (stale docs, dead-end directories, uncommitted knowledge) is a compound risk. It makes each subsequent sprint slower. The Lead Engineer's discipline around clean commits and current documentation is the mitigation.

---

## How to evaluate a new risk

When a situation arises that is not covered by this document, evaluate it against two questions:

1. Is the downside bounded? (Can we stop the bleeding if it goes wrong?)
2. Is the decision reversible? (Can we undo it if it turns out to be a mistake?)

If yes to both: accept the risk and proceed. If no to either: slow down, name the risk explicitly in NEXT_ACTIONS.md as a Needs Ryan item, and get Ryan's approval before proceeding.

---

## Version history

| Version | Date | Change |
|---------|------|--------|
| 1.0 | 2026-07-09 | Initial risk framework |
