# Offer Design — ADA Website Compliance Monitoring

**Experiment:** Experiment Zero
**Step:** 4 (Offer Design)
**Owner:** Offer and Lead Gen Strategist
**Date:** 2026-07-09
**Status:** COMPLETE

---

## The One-Sentence Value Proposition

We scan your website every month for ADA violations, send you a plain-English report showing exactly what is broken and what to fix, so you can reduce your lawsuit exposure without paying a lawyer or hiring a developer just to find out the problem.

---

## Offer Name

**ClearPath ADA Monitor**

Reasoning: "Clear" signals plain-language reporting (our differentiator). "Path" signals direction and fixability. "ADA Monitor" is descriptive for search and cold outreach. Not a made-up word. Not trademarked by a direct competitor.

---

## What the Customer Gets

**Every month:**
- Automated WCAG 2.1 AA scan of all pages on their website
- Plain-English violation report (PDF + web view) showing: violation type, which page, severity (Critical / Serious / Moderate), and a plain-English fix description
- Risk score: Low / Medium / High / Critical based on violation severity and count
- Month-over-month comparison: Did anything get worse? Did fixes stick?

**On signup:**
- Initial full-site audit (same format as monthly reports)
- Baseline risk score with context: "Sites with this profile have a [X]% likelihood of receiving a demand letter based on industry data"
- Remediation priority list: The three fixes most likely to reduce lawsuit exposure first

**What is not included:**
- We do not fix the site. We tell the client what is broken.
- We do not provide legal advice.
- We do not use overlays or widgets.

This is deliberate. Fixing requires a developer. Offering to fix adds variable cost, human time, and legal exposure. Monitoring is a clean recurring product.

---

## Pricing

Two tiers. No monthly discounts — annual only for the lower price to improve cash collection.

| Tier | Monthly (month-to-month) | Annual (paid upfront) | Sites covered |
|------|--------------------------|-----------------------|---------------|
| Solo | $99/month | $990/year ($82.50/mo) | 1 site |
| Multi | $179/month | $1,790/year ($149/mo) | Up to 5 sites |

**Pricing rationale:**
- accessiBe charges $490/year ($41/month) for an overlay with credibility problems
- Our product is more credible and more useful than an overlay
- $99/month is $100 more per month than we need to exceed their price — but we are not competing on price
- $99/month is less than 4 hours of the cheapest attorney's time
- $990/year is less than 4% of a typical ADA lawsuit settlement
- The Multi tier creates a clear upgrade path and captures agencies managing client sites

**Free scan hook (acquisition only — not a tier):**
A free one-time compliance scan with a single-page summary report. This is the cold outreach mechanism. The report shows:
- Overall risk score
- Total violation count by severity
- Three examples of real violations found on their site
- What those violations could cost them

The free scan is not the product. It is the introduction. It demonstrates the value of the product in 30 seconds.

---

## Why Someone Chooses This Over accessiBe or UserWay

Specific answer: because accessiBe and UserWay use overlays, and overlays are being sued around.

A business owner who has done any research will find the Overlay Fact Sheet, the National Federation of the Blind's statements, or news about other businesses getting sued while using overlays. That research creates doubt about overlays that our product resolves completely — because we do not use overlays.

For the business owner who has not done that research, the positioning is simpler: we tell you what is actually broken. They tell you the problem is solved. We help you fix it. They cover it up.

The pitch is not technical. It is: "You paid for a smoke detector that beeps but doesn't call the fire department. We tell you where the fire is."

---

## The Free Scan Mechanic (Cold Outreach)

**How it works:**
1. Run an automated WCAG 2.1 AA scan on a prospect's domain (takes 2-5 minutes)
2. Generate a one-page report showing: total violation count, risk score, three specific violations with plain-English descriptions
3. Send the report as a PDF attachment in the cold email
4. Email subject: "Your site has [N] ADA violations — free compliance report attached"
5. Email body: The violations we found, what they could cost, how our monitoring prevents it, and a link to start a free 14-day trial

**Why this works:**
- The report is specific to their site, not generic
- It demonstrates the product before asking for money
- The violations are real — they are not manufactured. Most sites have dozens to hundreds of genuine violations.
- The fear trigger (lawsuit risk) is present, documented, and attached to their specific situation
- No pitch call required. The report does the selling.

**What is needed to run this at scale:**
- An automated scanning tool (open source options: axe-core, Pa11y, Lighthouse accessibility audit)
- A report generation template (PDF output)
- An email sending system (cold email tool: Instantly, Apollo, Lemlist, or similar)
- A prospect list from Apollo.io or Hunter.io

All of this is operational infrastructure, not development. The validation test runs manually for the first 100 prospects.

---

## What Happens After a Client Signs Up

1. Client provides their URL(s)
2. System runs initial full-site scan (automated)
3. Initial audit report delivered within 24 hours
4. Monthly recurring scans run automatically
5. Monthly report sent via email
6. Client accesses reports via simple web portal (future state — validation uses email delivery only)

Ryan's time after client signup: approximately 5 minutes per new client to add them to the scanning queue. Less after automation is built.

---

## Honest Assessment of This Offer

**Strengths:**
- Recurring revenue, no human fulfillment after scan automation is built
- Real problem, documented legal risk, identifiable buyer
- Price justified by risk reduction math, not competitive comparison
- Free scan acquisition model is unusual in this market and easy to personalize

**Risks:**
- Building the scanning and report generation infrastructure takes development time and money before the first dollar
- Validation requires a working scan + report pipeline even for the test
- If overlay companies improve their product or the legal environment shifts, differentiation weakens
- The fix-it-yourself model requires client sophistication — some clients will expect us to fix the violations and be disappointed

**Validation consideration:** The 7-day validation test does not require a fully built product. It requires a working free scan + real report to send to prospects, and a believable landing page or pitch. If 3+ people express genuine buying interest based on the free scan, the product is worth building.
