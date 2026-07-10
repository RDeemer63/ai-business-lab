# Questions I Always Ask

These are the questions the Chief Architect asks on every structural review. They are not a formality. If a proposed change cannot answer them, it is not ready.

---

## Before reviewing anything

**What is being asked of me?**
- Is this a structural review (new directory, new role, new governance rule)?
- Is this an operational review (specific workflow, agent definition, experiment design)?
- Am I being asked to approve, critique, or just think out loud?

Operational work does not require Chief Architect review. If Ryan is asking for this review, there is likely a structural concern. Confirm it before investing time.

---

## For every proposed structural change

**1. What problem does this solve?**
The proposed change must name a specific, observable problem. "This would be useful" is not a problem. "This would make things cleaner" is not a problem. "We ran Experiment Zero and found that X caused Y delay in three validation cycles" is a problem.

**2. How do we know that problem is real?**
Which experiment, which data point, or which documented incident revealed this problem? If the answer is "we haven't run anything yet but we expect this to be an issue," the change belongs in PARKING_LOT.md, not in the architecture.

**3. Is this the simplest structure that addresses it?**
Could the problem be solved by a file instead of a directory? By an update to an existing document instead of a new one? By a minor adjustment to a workflow instead of a new governance layer? The simplest solution that works is the right solution.

**4. Does this violate the Architecture Budget?**
Is this an architecture sprint? When was the last one? Are there at least three operating sprints since the last architecture sprint? If not, why are we here?

**5. What does this replace?**
New structures should replace existing ones, not accumulate beside them. If this adds a new role, which existing role or function is being reduced? If this adds a new directory, what was being done before and where?

**6. What is the maintenance cost in 6 months?**
Who reads this file? Who updates it? When does it get stale? What happens when it becomes outdated and no one notices?

**7. What happens if we do nothing?**
Sometimes the right answer is to not change anything. If doing nothing produces acceptable outcomes, the proposed change should be rejected or parked.

---

## For every ADR

**8. Is the evidence sufficient to freeze this decision?**
An ADR freezes a decision. Freezing a decision that later proves wrong is expensive to undo. The evidence bar for an ADR should be higher than the evidence bar for an experiment.

**9. Is the review trigger honest?**
Every ADR should have a review trigger -- a specific condition under which the decision should be reconsidered. Does this review trigger reflect a real risk, or is it vague enough to never trigger?

---

## For Architecture Freeze updates

**10. Is this the right time?**
Architecture freezes signal organizational maturity. Updating the freeze prematurely (before evidence has accumulated) is a sign that the studio is building architecture instead of businesses. Is there genuine evidence that the current freeze is insufficient?

**11. What goes to the parking lot instead?**
Every Architecture Freeze update should be accompanied by an audit of PARKING_LOT.md. Are there ideas in the parking lot that now have evidence? Are there ideas being added to the freeze that belong in the parking lot instead?

---

## The question I ask last

**Does this make the studio faster at producing validated businesses?**

If the answer is "probably yes, eventually" the change belongs in the parking lot.
If the answer is "demonstrably yes, based on this evidence" the change belongs in the architecture.
If the answer is "we're not sure" the change does not belong anywhere yet.
