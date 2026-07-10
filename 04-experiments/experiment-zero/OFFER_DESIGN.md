# Offer Design — Website Accessibility Monitoring

**Experiment:** Experiment Zero
**Step:** 4 (Offer Design)
**Owner:** Offer and Lead Gen Strategist
**Date:** 2026-07-09
**Status:** COMPLETE — repositioned 2026-07-09 per Issue #4

> **Disclaimer:** Automated testing detects only some accessibility barriers and does not determine legal compliance. This report is not legal advice and does not guarantee protection from claims.

---

## The One-Sentence Value Proposition

We scan your website every month for accessibility issues, send you a plain-English report showing exactly what is broken and what to fix first, so you know what needs attention without paying a developer or a lawyer to find out.

---

## Offer Name

**ClearPath Accessibility Monitor**

Reasoning: "Clear" signals plain-language reporting (our differentiator). "Path" signals direction and fixability. "Accessibility Monitor" is accurate and descriptive. Not trademarked by a direct competitor.

Note: Previous name was "ClearPath ADA Monitor." Renamed to remove the implication that automated scanning determines ADA compliance or legal standing.

---

## What the Customer Gets

**Every month:**
- Automated WCAG 2.1 AA scan of their website
- Plain-English violation report showing: issue type, which page, severity (Critical / Serious / Moderate), and a plain-English description of what to fix
- Accessibility score: Low / Medium / High / Critical based on violation severity and count
- Month-over-month comparison: Did anything get worse? Did fixes stick?

**On signup:**
- Initial full-site scan (same format as monthly reports)
- Remediation priority list: The three issues most likely to create friction for users with disabilities

**What is not included:**
- We do not fix the site. We tell the client what is broken.
- We do not provide legal advice.
- We do not use overlays or widgets.
- We do not guarantee compliance with any law or regulation.

> Automated testing detects only some accessibility barriers and does not determine legal compliance. This report is not legal advice and does not guarantee protection from claims.

This scope is deliberate. Fixing requires a developer. Offering to fix adds variable cost, human time, and liability. Monitoring is a clean recurring product.

---

## Pricing

Two tiers. Month-to-month or annual.

| Tier | Monthly (month-to-month) | Annual (paid upfront) | Sites covered |
|------|--------------------------|-----------------------|---------------|
| Solo | $99/month | $990/year ($82.50/mo) | 1 site |
| Multi | $179/month | $1,790/year ($149/mo) | Up to 5 sites |

**Pricing rationale:**
- accessiBe charges $490/year ($41/month) for an overlay product
- Our product is a different category — monitoring, not overlays
- $99/month is less than one hour of attorney time at most law firms
- Annual option improves cash collection and rewards commitment

---

## Why Someone Chooses This Over accessiBe or UserWay

Specific answer: because accessiBe and UserWay use overlays, and overlays have a documented credibility problem.

The Overlay Fact Sheet (a publicly available document signed by hundreds of accessibility professionals) states that overlays do not solve accessibility problems and may introduce new ones. The National Federation of the Blind has issued critical statements about overlays. Several businesses have been sued while using overlays, because the underlying site content remained inaccessible.

Our product does not use overlays. We tell the client what is actually broken. They tell you the problem is solved. We help you understand what to fix. They cover up the symptoms.

The pitch is not technical. It is: "You paid for a smoke detector that beeps but does not call the fire department. We tell you where the fire is."

---

## The Free Scan Mechanic (Cold Outreach)

**How it works:**
1. Lead Engineer runs an automated WCAG 2.1 AA scan on the prospect's domain using a batch scanner (Pa11y, axe-core, or Lighthouse CLI)
2. Scanner outputs a one-page HTML report: issue count by severity, three specific examples with plain-English descriptions
3. Report is hosted at a URL and linked in the cold email (not attached as PDF — see Fix 4 in Issue #4)
4. Email subject: "We found [N] accessibility issues on [domain] — free report"
5. Email body: What we found, three specific examples, what the service does, link to the report

**What makes this work:**
- The report is about their actual site, not a generic pitch
- It demonstrates the product before asking for money
- The issues are real — most sites have detectable WCAG failures
- The call to action is simple: "Want us to monitor this monthly so you stay current?"

**What is needed before Day 1:**
- Lead Engineer builds the batch scanner + HTML report generator (separate task, before Day 0)
- Dedicated sending domain set up and warmed (see VALIDATION_PLAN.md)
- Prospect list from Apollo.io

---

## Honest Assessment of This Offer

**Strengths:**
- Recurring revenue, no human fulfillment after automation is built
- Real problem, identifiable buyer, specific product
- Free scan acquisition mechanic is unusual and personalizable
- No-overlay positioning differentiates cleanly from the market leaders

**Risks:**
- Building the scanning and report generation infrastructure takes time before the first dollar
- Some prospects will want us to fix the violations, not just report them — the scope limitation will disappoint them
- Accessibility monitoring without legal compliance claims is a harder sell than fear-based marketing, but it is the accurate sell

**Validation note:** The 7-day test does not require a fully built product. It requires a working batch scanner, a report for each prospect, a hosted report URL, and a plain-English email. If 3+ people ask about pricing, a call, or how to sign up, the offer is worth building.
