# Validation Plan — Website Accessibility Monitoring

**Experiment:** Experiment Zero
**Step:** 5 (Validation Plan — REVISED — PENDING RYAN APPROVAL v2)
**Owner:** Chief of Staff
**Date:** 2026-07-09
**Status:** REVISED — PENDING RYAN APPROVAL (v2) — do not proceed to Step 6 until approved

> **Disclaimer:** Automated testing detects only some accessibility barriers and does not determine legal compliance. This report is not legal advice and does not guarantee protection from claims.

---

## Revision Log

| Version | Date | Changes |
|---------|------|---------|
| v1 | 2026-07-09 | Initial draft |
| v2 | 2026-07-09 | Revised per Issue #4: repositioned product language (ADA compliance removed), corrected legal claims in MARKET_RESEARCH.md, removed manual scanning from Ryan's scope (Lead Engineer builds batch scanner before Day 0), added dedicated sending domain requirement, strengthened success signal with full funnel tracking, changed hook to factual version |
| v3 | 2026-07-09 | Chief Architect Stage Gate: KPI held at under 2 hours — email workflow redesigned so agents prepare all 100 drafts, Ryan spot-checks 5 and approves batch send. "Violation report" changed to "accessibility issue report" throughout. |

---

## What This Plan Authorizes

Ryan's approval of this plan authorizes Step 6: Outbound Strategist writes the cold email, subject line, and follow-up sequence. Ryan reviews and approves those messages before any email is sent.

Ryan's approval of this plan does NOT authorize sending any emails. That gate happens at Step 6.

---

## The Test

Can ClearPath Accessibility Monitor produce at least one concrete commitment (or 3+ genuine interest replies) from strangers in 7 days, using a personalized free accessibility scan as the hook?

This is not a test of whether website accessibility monitoring is a good business in the abstract. It is a test of whether this specific offer, at this specific price, reaching this specific buyer through this specific channel, produces a go signal.

---

## Target Customer

**Who receives the email:**

Job title: Owner, Co-Owner, Practice Manager, Office Manager, Marketing Manager

Company type: Small business with a physical location and a website. Industries with documented high rates of website accessibility litigation: restaurants, medical and dental practices, retail stores, hotels and lodging, professional services.

Company size: 5-50 employees. Large enough to have a web presence. Small enough to not have a dedicated legal or IT team.

Revenue: Estimated $500K-$5M annually. Can approve a $99/month expense without a committee.

Geography: United States. California, New York, Florida, Texas weighted first (highest ADA filing activity per UsableNet data).

**Why this buyer:**
- Has a website they did not build themselves and cannot easily modify
- Is in an industry with documented accessibility lawsuit activity
- Has the authority and budget to say yes without a long approval process

---

## The Hook

**Version tested (v1 — factual):**

> We found [N] automated accessibility issues on [domain], including [three specific examples]. We created a free plain-English report showing what to review and prioritize.

**Why the factual version:**
The fear-based hook ("You have [N] ADA violations that could expose you to a lawsuit") overstates what an automated scan can establish. Automated tools detect a subset of WCAG failures — they do not determine legal compliance or lawsuit exposure. Using that framing in outreach copy creates legal risk for the studio and is inaccurate.

The factual version is being tested as Hypothesis A: that the value of the scan itself (specific, personalized, plain-language) is compelling without a fear trigger. If this hook underperforms, a refined second iteration can test urgency framing. We start with the accurate version.

**The free scan is real.** The Lead Engineer's batch scanner runs an actual WCAG 2.1 AA scan on each prospect's domain. The report shows real issues on their specific site. It is not a generic pitch.

---

## Pre-Test Requirements (Day 0)

The following must be complete before Day 1 emails go out:

- [ ] Lead Engineer builds and tests the batch scanner + HTML report generator. Accepts a list of URLs, outputs one hosted report URL per domain. Ryan does not run scans manually.
- [ ] Dedicated sending domain registered (e.g., getclearpath.co or similar — not Ryan's primary domain)
- [ ] New dedicated mailbox set up on the sending domain
- [ ] SPF, DKIM, and DMARC configured and verified on the sending domain
- [ ] Sending domain warmed for at least 7 days before Day 1
- [ ] Prospect list of 100 contacts built in Apollo.io and reviewed by Ryan
- [ ] Sample scan report reviewed by Ryan (confirm format is clear and credible)
- [ ] Step 6 completed: Outbound Strategist writes email, Ryan approves

---

## Channel

**Primary:** Cold email

**List source:** Apollo.io

Filter criteria:
- Industry: Restaurants, medical/dental, retail, professional services, hotels
- Company size: 5-50 employees
- Geography: CA, NY, FL, TX weighted first
- Job title: Owner, Practice Manager, Office Manager, Marketing Manager

**List size:** 100 prospects

**Email delivery:** Sent from the dedicated sending domain and mailbox. Not Ryan's primary email. Reports delivered via hosted link, not PDF attachment (better deliverability, avoids spam filter triggers from attachments).

---

## Timeline

| Day | Action | Who |
|-----|--------|-----|
| Day 0 (pre-test) | Ryan approves this plan. All pre-test checklist items complete. Agents deliver 100 prepared email drafts for Ryan's review. | Ryan + Lead Engineer + Agents |
| Day 0 | Ryan spot-checks 5 email drafts. Approves batch. Batch send triggered from dedicated mailbox. | Ryan |
| Day 1-2 | Monitor inbox for replies. Log any responses as they arrive. | Ryan |
| Day 3-4 | Reply to any responses. Classify interest level. | Ryan |
| Day 5 | Agents prepare follow-up drafts for non-responders. Ryan approves and triggers batch follow-up. | Ryan + Agents |
| Day 6 | Agents prepare follow-up drafts for Day 2 batch. Ryan approves and triggers. | Ryan + Agents |
| Day 7 | Count and classify all responses. | Ryan |
| Day 7 (evening) | Report results to Chief of Staff. Step 8 begins. | Ryan |

---

## Funnel Tracking

Track every metric. Record in RYAN_TIME_LOG.md.

| Metric | Target | Actual |
|--------|--------|--------|
| Emails sent | 100 | |
| Emails delivered (bounces subtracted) | | |
| Opens (if tracking enabled) | | |
| Replies (any) | | |
| Replies classified as genuine interest | | |
| Calls or demos requested | | |
| Trials explicitly requested | | |
| Concrete commitments (paid pilot, deposit, card auth, explicit trial start with business info supplied) | | |

---

## Signal Definitions

**Strong go signal:** At least 1 concrete commitment within 7 days — paid pilot, deposit, card authorization, or explicit trial start with business information provided. Build.

**Moderate go signal:** 3 or more genuine interest replies with no concrete commitment. Warrants a second iteration with a refined message before build decision. Do not build on moderate signal alone.

**Inconclusive:** 1-2 genuine interest replies. Second iteration recommended. Not a go.

**No-go:** Fewer than 3 genuine interest replies after the full 7 days including follow-up sequence. Document, post-mortem, redirect.

**Definition of Genuine Interest:** The prospect asks about pricing, asks how to sign up, requests a call or demo, or says they want to learn more. Polite acknowledgment ("thanks for the report") does not count.

---

## Failure Classification

If we hit no-go, determine which kind of failure occurred before deciding whether to try again:

| Failure type | Indicator | What it means |
|-------------|-----------|--------------|
| Channel failure | Open rate very low or zero, few bounces | Prospect list wrong, or sending domain issue |
| Message failure | Opens but no replies | Hook did not land, or subject line did not pull |
| Offer failure | Replies but rejections | Prospects understand the product and said no |
| Inconclusive | Some interest but not enough signal | Second iteration warranted |

If open tracking is unavailable, channel vs. message failure is harder to distinguish. Note this limitation in the post-mortem.

---

## Ryan's Role and Time Budget

Ryan's time recalculated with manual scanning and email drafting both off his plate.

| Task | Estimated time |
|------|---------------|
| Review this plan (Step 5) | 15 minutes |
| Review sample scan report format | 10 minutes |
| Review and approve prospect list | 15 minutes |
| Review and approve cold email template (Step 6) | 15 minutes |
| Spot-check 5 prepared email drafts, approve batch send | 10 minutes |
| Monitor inbox and log replies Days 1-4 | 10 minutes total |
| Approve follow-up batch (Days 5-6) | 5 minutes |
| Report results to Chief of Staff Day 7 | 10 minutes |
| Review go/no-go recommendation (Step 8) | 15 minutes |

**Total estimated Ryan time: 1 hour 45 minutes maximum**

Agents prepare all 100 personalized email drafts before Day 0. Each draft is pre-filled with the prospect's domain, issue count, and three specific accessibility issues from the batch scan. Ryan spot-checks 5, approves the batch, and the send is triggered. Ryan does not copy, paste, or manually send 100 individual emails.

The dedicated sending domain setup, scanner build, and draft preparation are Lead Engineer and agent tasks. They do not count against Ryan's budget.

---

## Definition of Done for This Plan

Step 5 is complete when Ryan approves this plan (adds name and date below).

All five revised criteria per Issue #4 are met:
1. Legal and market claims are corrected and sourced (MARKET_RESEARCH.md v2)
2. Product language separates automated accessibility testing from legal compliance
3. Ryan's estimated time is under 2h20m with no manual scanning assigned to him
4. Sending setup protects Ryan's primary domain
5. Success criteria include a strong commitment signal

**Ryan Approval:**

Name: ____________________________
Date: ____________________________
Approved as written / Approved with the following changes:

_________________________________________________________

---

## Stop Condition

Reconsider this plan before Step 6 if:
- The batch scanner build reveals a technical blocker that prevents automated report generation
- The dedicated sending domain cannot be warmed in time for the planned test window
- A material change in the legal landscape (DOJ action on Title III, major court ruling) changes the accuracy of the marketing framing before the test begins
- Ryan's schedule does not allow 30-45 minutes on Day 1 and Day 2 for email sending

If any stop condition is met, flag to Ryan before proceeding.
