# Outreach Draft — Experiment Zero

**Product:** ClearPath Accessibility Monitor
**Step:** 6 (Outbound Strategist)
**Status:** PENDING RYAN APPROVAL — do not send until approved
**Date:** 2026-07-09

Ryan must review and approve all messages in this document before any email is sent. This is the final gate before execution begins.

---

## Section 1: Subject Line Variants

**A (Recommended):** `Free accessibility report for [DOMAIN]`

**B:** `We scanned [BUSINESS_NAME]'s website — here's what we found`

**C:** `[ISSUE_COUNT] accessibility issues on [DOMAIN] — free report inside`

See Section 5 for the recommendation rationale.

---

## Section 2: Primary Cold Email (v1 — Factual Hook)

**Subject:** [Use chosen variant from Section 1]

---

Hi [FIRST_NAME],

We ran an automated accessibility scan of [DOMAIN] and found [ISSUE_COUNT] issues that affect how some visitors experience your site.

Three examples from your site:

- [EXAMPLE_1]
- [EXAMPLE_2]
- [EXAMPLE_3]

Here's the free report: [REPORT_LINK]

It shows the full list, sorted by severity, with plain-English notes on what each issue is.

If you want us to scan your site every month and send you a report like this — so you always know where things stand — reply and I'll get it set up. It's $99 a month.

No pressure either way. The report is yours regardless.

Ryan
ClearPath Accessibility Monitor

---

**Word count:** ~110 words

**What this email does and does not do:**
- Opens with what we found on their specific site, not a generic pitch
- Gives three real examples in plain English before asking for anything
- One clear primary CTA: the report link
- One soft secondary CTA: reply to start monitoring
- Makes no legal claims
- Disclaimer lives on the report page, not in the email body

---

## Section 3: Follow-Up Email (Day 5-6, Non-Responders)

**Subject:** Re: [original subject line thread]

---

Hi [FIRST_NAME],

Following up on the report I sent earlier.

One thing worth noting: the issues we found don't fix themselves. Most of them have been there since the site was built. The report at [REPORT_LINK] shows exactly which ones are worth prioritizing first.

If you have five minutes to look it over, I'm happy to answer any questions.

Ryan

---

**Word count:** ~60 words

**Notes:** This is sent as a reply to the original thread, so it inherits context. Gives one new observation (issues don't fix themselves, implies this is worth acting on) without repeating the pitch or adding pressure.

---

## Section 4: Merge Field Reference

| Field | Contents | Source |
|-------|----------|--------|
| [FIRST_NAME] | Prospect's first name | Apollo.io contact record |
| [BUSINESS_NAME] | Business name | Apollo.io company record |
| [DOMAIN] | Website domain (e.g., smithdentalcare.com) | Apollo.io company record |
| [ISSUE_COUNT] | Total accessibility issues found by the batch scanner | Batch scanner output per domain |
| [EXAMPLE_1] | First priority issue, written in plain English | Batch scanner output — see personalization notes in Section 5 |
| [EXAMPLE_2] | Second priority issue, written in plain English | Batch scanner output |
| [EXAMPLE_3] | Third priority issue, written in plain English | Batch scanner output |
| [REPORT_LINK] | Hosted URL to the one-page HTML report for this domain | Lead Engineer batch scanner output |

**Important:** [EXAMPLE_1], [EXAMPLE_2], [EXAMPLE_3] are the three highest-severity issues found on that specific domain. They must be written in plain English before being inserted into the email. See Section 5 for how to do this.

---

## Section 5: Sending Notes

### Subject line recommendation

**Start with Subject A:** `Free accessibility report for [DOMAIN]`

Rationale: It is specific (uses their domain), it leads with the gift (a free report), and it is not clickbait. "Free" in subject lines can trigger spam filters in some sending configurations — if deliverability testing shows filter problems, switch to Subject B. Subject C with the issue count is the most specific but may read as sensationalized to some recipients; reserve it for a second iteration if A underperforms.

### Recommended send time

Tuesday, Wednesday, or Thursday. Between 7:30-9:00 am local time for the prospect's time zone, or 1:00-2:30 pm. Avoid Monday (inbox overload) and Friday (mentally checked out).

For the first batch of 100, send Tuesday-Wednesday morning to maximize the response window within the 7-day test period.

### Plain text vs. HTML

**Send plain text only.**

Reasons:
- Higher deliverability from a new sending domain — HTML emails are more likely to land in promotions or spam tabs
- Plain text reads as a personal email, not a blast
- The report link carries the visual presentation; the email itself does not need formatting
- Easier to read on mobile

No images, no logo, no signature banner. Just text and a link.

### How to write the three plain-English issue examples

The batch scanner outputs WCAG technical identifiers. Before inserting into the email, translate each one into a plain-English sentence a business owner can understand without technical background. The sentence should describe what the issue is and why it matters to a real user.

**Translation examples:**

| Scanner output | Email copy |
|---------------|-----------|
| Missing alt text on 12 images | 12 images on your site have no text description, so visitors using screen readers hear nothing when they encounter them |
| Low color contrast on navigation links | Your navigation links are hard to read for people with low vision — the text and background colors are too similar |
| Form submit button has no accessible label | Your contact form's submit button has no label, so screen reader users cannot tell what it does |
| Missing page title on 3 pages | Three pages on your site have no title, which makes navigation confusing for keyboard and screen reader users |
| Videos have no captions | Your embedded videos have no captions, which excludes visitors who are deaf or hard of hearing |

**Rule:** If you cannot explain the issue in one sentence that a restaurant owner would understand, rewrite it. Do not include technical terms in the email body.

### Pre-send checklist

Before Ryan approves and triggers the batch:

- [ ] All 100 email drafts have been generated by agents with real merge field values filled in
- [ ] [EXAMPLE_1], [EXAMPLE_2], [EXAMPLE_3] have been translated to plain English for each domain
- [ ] All [REPORT_LINK] values point to live hosted report URLs (not broken links)
- [ ] Ryan has spot-checked at least 5 drafts and confirmed they read naturally
- [ ] Sending domain is warmed and SPF/DKIM/DMARC are verified
- [ ] Send time is scheduled for Tuesday or Wednesday morning
