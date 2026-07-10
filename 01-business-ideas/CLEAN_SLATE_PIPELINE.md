# Clean Slate Idea Pipeline — Track B

**Date:** 2026-07-09
**Prepared by:** Chief of Staff
**Method:** Founder-history bias eliminated. Ideas generated without reference to Ryan's existing companies, audiences, industries, or software. Founder advantage excluded from first-pass scoring.

---

## Scoring Methodology

**First-pass criteria (no founder input):**

| Code | Criterion | 5 = best |
|------|-----------|----------|
| S1 | Speed to first dollar | First paying customer within 2 weeks |
| S2 | Automation potential | Operations require zero human intervention |
| S3 | Gross margin | 90%+ margin |
| S4 | Recurring revenue potential | Monthly billing, high LTV |
| S5 | Customer-support burden | Customers rarely contact you |
| S6 | Sales complexity | Customers self-serve or buy from a short email |
| S7 | Operational complexity | Running the service requires no specialized expertise |
| S8 | Market urgency | Customers feel acute pain and actively seek solutions |
| S9 | Competitive intensity | Few direct competitors at the price point |
| S10 | Sub-5-hours/week operability | Fully manageable in under 5 hours/week post-launch |

**Weighted score formula:**
`(S1 + S5 + S6 + S7 + S8 + S9) + 1.5 × (S2 + S3 + S4 + S10)`
Max = 60. Weighted criteria: S2, S3, S4, S10.

**Second-pass Ryan fit (top 10 only):**

| Code | Criterion | 5 = best |
|------|-----------|----------|
| F1 | Market legibility | Ryan could fully understand this market within 30 days |
| F2 | Transferable skills | His current skills apply directly |
| F3 | Distribution advantage | Access to early customers through existing channels |
| F4 | Distraction risk | Low risk of pulling focus from current businesses |

Ryan fit score = F1 + F2 + F3 + F4 (max 20). Does not change business quality score.

---

## Full Pipeline — All 30 Ideas Ranked

| Rank | Idea | Weighted Score |
|------|------|---------------|
| 1 | Automated Job Description Bias Checker | 54.5 |
| 2 | ADA Website Compliance Monitoring | 54 |
| 3 | Privacy Policy & Cookie Consent Monitor | 54 |
| 4 | Automated Contract Redline Summarizer | 53.5 |
| 5 | SOC 2 Evidence Collection Template Pack | 53.5 |
| 6 | AI-Powered Employee Handbook Generator | 52.5 |
| 7 | Government Contract Award Monitor | 52 |
| 8 | Automated Review Request Service (E-Commerce) | 52 |
| 9 | SaaS Tool Replacement Finder | 50.5 |
| 10 | Permit Expiration Alert Service | 50 |
| 11 | Price Tracking & Competitive Intel (E-Commerce) | 50 |
| 12 | Financial Model Template Library | 49.5 |
| 13 | AI Prompt Library Subscription | 49.5 |
| 14 | Regulatory Change Digest (SaaS Compliance) | 49 |
| 15 | OSHA Compliance Document Generator | 48.5 |
| 16 | Job Posting Trend Monitor | 47.5 |
| 17 | AI-Powered RFP Response Generator | 46.5 |
| 18 | B2B Benchmark Report Subscriptions by Role | 46.5 |
| 19 | AI Agent Prompt Framework License | 45.5 |
| 20 | Commercial RE Permit & Zoning Intelligence Feed | 45.5 |
| 21 | Competitive Landscape Reports for VC Associates | 44 |
| 22 | Independent Insurance Agency Finder | 44 |
| 23 | Verified Franchise Opportunity Directory | 43 |
| 24 | Verified M&A Advisor Directory | 42.5 |
| 25 | White-Label AI Report Generator | 42 |
| 26 | Niche Industry Salary Benchmarking Reports | 41 |
| 27 | Market Entry Analysis Reports for B2B SaaS | 40 |
| 28 | B2B Software Vendor Comparison Aggregator | 39 |
| 29 | Verified Expert Marketplace for Compliance | 36 |
| 30 | Micro-Consulting Marketplace | 29 |

---

## Top 10 — Full Profiles

---

### 1. Automated Job Description Bias Checker
**Business quality score: 54.5 / 60**
**Ryan fit score: 11 / 20**

#### Scoring Table

| Criterion | Score | Notes |
|-----------|-------|-------|
| S1 Speed to first dollar | 5 | Launch a free tool on ProductHunt or Hacker News; paid tier converts immediately |
| S2 Automation potential (×1.5) | 5 | LLM classification of bias patterns is fully automated; no human review needed |
| S3 Gross margin (×1.5) | 5 | Pure software; near-zero marginal cost |
| S4 Recurring revenue (×1.5) | 4 | Monthly subscription works; some users buy one-time for a project |
| S5 CS burden | 5 | Results are self-explanatory; no support queue |
| S6 Sales complexity | 5 | Free tool + self-serve upgrade; no sales call required |
| S7 Operational complexity | 5 | LLM API call + result display; nothing to manage |
| S8 Market urgency | 4 | DEI pressure on HR teams is real but not emergency-level |
| S9 Competitive intensity | 2 | Textio, Gender Decoder, and Ongig compete; differentiation requires a clear angle |
| S10 Sub-5-hours/week (×1.5) | 5 | Fully automated after launch |

**Weighted score:** (5+5+5+5+4+2) + 1.5×(5+5+4+5) = 26 + 28.5 = **54.5**

#### Ryan Fit Table

| Fit Criterion | Score | Notes |
|--------------|-------|-------|
| F1 Market legibility | 3 | HR tech is learnable but Ryan has no grounding in it; 30 days is tight |
| F2 Transferable skills | 3 | AI pipeline and technical ops apply; HR domain knowledge does not |
| F3 Distribution advantage | 1 | Zero overlap with existing contractor/agency audience |
| F4 Distraction risk | 4 | Completely separate from current businesses |

**Ryan fit: 11 / 20**

**Customer:** HR managers and recruiters at companies with 50-500 employees under pressure to improve hiring diversity metrics.

**Painful problem:** Biased job descriptions reduce the qualified candidate pool and create legal exposure. HR teams know this but lack a fast, cheap tool to audit at scale.

**Offer:** Paste any job description, receive an instant bias analysis flagging gendered language, experience inflation, unnecessary requirements, and cultural exclusion signals. Suggested rewrites included. Paid tier adds bulk upload and team reporting.

**Pricing:** Free (1 check/day) | $49/month (unlimited) | $199/month (team + reporting)

**Revenue math to $5k/month:** 102 individual subscribers at $49 or 26 team subscribers at $199

**Revenue math to $10k/month:** 204 individual or 51 team subscribers

**Sales motion:** Free tool drives organic search ("job description bias checker"). ProductHunt and Hacker News launch drives initial spike. Paid upgrade is in-product. No outbound required.

**Fulfillment workflow:**
1. User pastes job description into web form
2. Text sent to Claude API with bias detection prompt
3. Structured analysis returned (flagged phrases, bias category, rewrite suggestions)
4. Results displayed instantly; download PDF for paid users
5. Monthly billing handled by Stripe

**AI agent roles:** Bias classification, pattern flagging, rewrite generation, report formatting, churn prediction from usage data.

**Human work before stabilization:** 60-80 hours — build the web form, integrate Claude API, design the output format, set up billing and free-tier limits, write documentation.

**Human work after stabilization:** 1-2 hours/week — monitor for prompt failures, review flagged edge cases, update prompt for new bias patterns as research evolves.

**Largest hidden bottleneck:** The bias detection model needs extensive prompt tuning before the output is good enough to charge for. Generic LLM responses are not specific enough — getting to "confident, consistent, auditable" output requires 40-60 hours of testing and iteration that looks invisible from the outside.

**7-day validation test:** Build a basic demo using Claude API (1 day). Post it on Hacker News and r/recruiting with "I built a free bias checker — feedback welcome." Track how many people use it and whether anyone asks about a paid version within 7 days.

---

### 2. ADA Website Compliance Monitoring
**Business quality score: 54 / 60**
**Ryan fit score: 15 / 20**

#### Scoring Table

| Criterion | Score | Notes |
|-----------|-------|-------|
| S1 Speed to first dollar | 4 | Free scan hook works fast; first paid subscriber possible within a week |
| S2 Automation potential (×1.5) | 5 | Automated scan via aXe/WAVE API + report generation; zero human touch |
| S3 Gross margin (×1.5) | 5 | Software scan + PDF report; near-zero marginal cost |
| S4 Recurring revenue (×1.5) | 5 | Monthly monitoring is the core value; site changes create ongoing issues |
| S5 CS burden | 4 | Reports are readable; occasional questions about specific violations |
| S6 Sales complexity | 4 | Free scan delivered by cold email is a proven hook; no call required |
| S7 Operational complexity | 4 | Once pipeline is built; data sources are stable |
| S8 Market urgency | 5 | ADA demand letters are real, daily, and expensive — this is fear-driven buying |
| S9 Competitive intensity | 3 | AccessiBe and AudioEye compete at premium; under $200/month is open |
| S10 Sub-5-hours/week (×1.5) | 5 | Scans run on schedule; reports generate and send automatically |

**Weighted score:** (4+4+4+4+5+3) + 1.5×(5+5+5+5) = 24 + 30 = **54**

#### Ryan Fit Table

| Fit Criterion | Score | Notes |
|--------------|-------|-------|
| F1 Market legibility | 4 | ADA compliance basics are learnable in a week; the law is well-documented |
| F2 Transferable skills | 4 | Technical pipeline, AI report generation, and selling to SMBs all apply directly |
| F3 Distribution advantage | 3 | Ryan's existing agency and contractor relationships are SMBs with websites |
| F4 Distraction risk | 4 | No overlap with core products; operates independently |

**Ryan fit: 15 / 20**

**Customer:** Small and mid-size business owners with websites who have received or fear receiving ADA demand letters (a common shakedown tactic targeting websites with accessibility violations).

**Painful problem:** ADA lawsuits against websites have surged. A single demand letter costs $5,000-$50,000 to resolve. Most business owners have no idea whether their site is compliant and no cheap way to find out.

**Offer:** Monthly automated accessibility scan of their website. Delivered as a PDF report listing every WCAG 2.1 violation, severity level, and specific element to fix. Includes a monthly compliance score and trend line. No remediation done — just the diagnostic.

**Pricing:** $97/month (1 site) | $197/month (up to 5 sites, for agencies)

**Revenue math to $5k/month:** 52 single-site subscribers or 26 agency subscribers

**Revenue math to $10k/month:** 103 single-site or 51 agency subscribers

**Sales motion:** Send a free unsolicited scan to a business owner's email: "I ran a free ADA scan on your site — you have 14 violations that could expose you to a lawsuit. Here's the report." No call required. They read the report, feel the fear, and click the subscribe link.

**Fulfillment workflow:**
1. Client domain added to system
2. Weekly/monthly scan runs via aXe-core API or similar
3. Violations parsed, categorized by severity (Critical, Serious, Moderate, Minor)
4. AI generates plain-English descriptions for each violation
5. PDF report assembled and emailed to client
6. Dashboard updated with compliance score history

**AI agent roles:** Violation description writing (converting technical WCAG codes to plain English), trend analysis, executive summary generation, follow-up email drafts for clients with critical violations.

**Human work before stabilization:** 60-80 hours — integrate scan API, build report generator, build billing, write cold email sequences, build onboarding flow.

**Human work after stabilization:** 1-2 hours/week — review reports flagged as anomalous, handle occasional billing issues, update violation database when WCAG standards update.

**Largest hidden bottleneck:** Cold email deliverability. The free scan hook requires sending unsolicited emails, which means domain reputation management, warm-up sequences, and bounce rate monitoring — all of which take longer to get right than the product itself.

**7-day validation test:** Pick 20 local businesses in one city. Run free scans on their sites using aXe (free). Write a one-paragraph plain-English summary of their worst violations. Send a cold email with the summary and a PDF. Track: how many open, how many reply, how many ask about ongoing monitoring.

---

### 3. Privacy Policy & Cookie Consent Compliance Monitor
**Business quality score: 54 / 60**
**Ryan fit score: 15 / 20**

#### Scoring Table

| Criterion | Score | Notes |
|-----------|-------|-------|
| S1 Speed to first dollar | 4 | Free scan hook plus immediate signup path |
| S2 Automation potential (×1.5) | 5 | Automated scanning and report generation; no human review |
| S3 Gross margin (×1.5) | 5 | Software only; near-zero marginal cost |
| S4 Recurring revenue (×1.5) | 5 | Monthly monitoring; regulations change, so re-checking is perpetual |
| S5 CS burden | 4 | Reports are self-explanatory; some questions about specific requirements |
| S6 Sales complexity | 4 | Free scan hook works; no call required |
| S7 Operational complexity | 4 | Once pipeline is built; regulatory updates require prompt maintenance |
| S8 Market urgency | 5 | GDPR, CCPA, and state privacy laws create real legal exposure with real fines |
| S9 Competitive intensity | 3 | Cookiebot and OneTrust dominate enterprise; under $200/month is underserved |
| S10 Sub-5-hours/week (×1.5) | 5 | Fully automated scans and reports |

**Weighted score:** (4+4+4+4+5+3) + 1.5×(5+5+5+5) = 24 + 30 = **54**

#### Ryan Fit Table

| Fit Criterion | Score | Notes |
|--------------|-------|-------|
| F1 Market legibility | 4 | GDPR/CCPA framework is learnable; surface-level compliance requirements are documented |
| F2 Transferable skills | 4 | Technical pipeline, AI report writing, SMB sales all directly applicable |
| F3 Distribution advantage | 3 | SMB and agency audience overlaps with existing contacts |
| F4 Distraction risk | 4 | Fully separate from current products |

**Ryan fit: 15 / 20**

**Customer:** Small business owners and marketing managers at companies with US or EU customers who collect any user data — which is nearly every website with a contact form or analytics tool.

**Painful problem:** Privacy regulations require specific disclosures, consent mechanisms, and policy language. Most small businesses copied a privacy policy from a template years ago and have never updated it. A single CCPA complaint to the AG can trigger an investigation and fines up to $7,500 per intentional violation.

**Offer:** Monthly automated privacy compliance scan. Checks: is the privacy policy present and current? Does it disclose data collection practices accurately? Is the cookie consent banner compliant with the regulations applicable to the site's audience? Delivered as a scored PDF report with specific gaps identified.

**Pricing:** $97/month (1 site) | $197/month (agency, up to 5 sites)

**Revenue math to $5k/month:** 52 single-site or 26 agency subscribers

**Revenue math to $10k/month:** 103 single-site or 51 agency subscribers

**Sales motion:** Free audit hook: "I scanned your site's privacy policy against current CCPA requirements — here are 3 gaps that could create liability." Email + report. No call. Signup link in the email.

**Fulfillment workflow:**
1. Scan site for privacy policy page, cookie consent banner, data collection signals
2. Classify findings against GDPR/CCPA checklist
3. AI generates plain-English gap descriptions with regulatory citations
4. PDF report assembled and delivered via email
5. Monthly rescan compares against previous report and flags new gaps

**AI agent roles:** Policy text analysis, cookie classification, gap identification, plain-language description writing, regulatory citation mapping, report assembly.

**Human work before stabilization:** 70-90 hours — build scan pipeline, write compliance checklist (requires legal research), build report generator, set up billing and onboarding.

**Human work after stabilization:** 2 hours/week — maintain compliance checklist as regulations update (this is the ongoing cost; regulations do change).

**Largest hidden bottleneck:** Regulatory accuracy. If the compliance checklist is wrong or outdated, the product gives false assurance, which creates real liability exposure. Getting the checklist right requires either deep legal research or a legal review — neither of which is fast or free.

**7-day validation test:** Hand-audit the privacy policies of 10 local businesses using a public CCPA compliance checklist. Write a one-paragraph gap summary for each. Email them with the summary and a PDF. Track responses and interest in ongoing monitoring.

---

### 4. Automated Contract Redline Summarizer
**Business quality score: 53.5 / 60**
**Ryan fit score: 14 / 20**

#### Scoring Table

| Criterion | Score | Notes |
|-----------|-------|-------|
| S1 Speed to first dollar | 4 | Quick demo possible; first paying user likely within a week |
| S2 Automation potential (×1.5) | 5 | LLM-powered; full contract analysis requires no human review |
| S3 Gross margin (×1.5) | 5 | Software; near-zero marginal cost |
| S4 Recurring revenue (×1.5) | 4 | Monthly subscription works; some users buy per-contract |
| S5 CS burden | 4 | Some edge cases with unusual contract structures |
| S6 Sales complexity | 4 | Self-serve SaaS; content marketing or paid search drives discovery |
| S7 Operational complexity | 5 | LLM API plus output formatting; nothing complex to maintain |
| S8 Market urgency | 5 | Every business owner who receives a vendor contract feels this pain |
| S9 Competitive intensity | 3 | Spellbook, LegalZoom, and Harvey compete at enterprise; affordable self-serve gap exists |
| S10 Sub-5-hours/week (×1.5) | 5 | Fully automated |

**Weighted score:** (4+4+4+5+5+3) + 1.5×(5+5+4+5) = 25 + 28.5 = **53.5**

#### Ryan Fit Table

| Fit Criterion | Score | Notes |
|--------------|-------|-------|
| F1 Market legibility | 4 | Business contracts are universal; no specialized legal expertise needed to build this |
| F2 Transferable skills | 4 | AI pipeline, technical ops, and writing all apply |
| F3 Distribution advantage | 2 | SMB audience overlaps broadly but Ryan has no specific channel to legal buyers |
| F4 Distraction risk | 4 | Separate from current businesses |

**Ryan fit: 14 / 20**

**Customer:** Founders, small business owners, and freelancers who receive vendor contracts, client agreements, partnership terms, or service agreements they don't want to pay a lawyer to review.

**Painful problem:** A $500/hour lawyer to review a vendor contract is not affordable for a $2M business. A non-lawyer reading a contract misses critical clauses. The gap between "sign without reading" and "pay for a lawyer" costs businesses money in bad deals.

**Offer:** Upload any contract PDF. Receive a structured plain-English summary covering: key obligations, payment terms, termination rights, liability exposure, non-standard clauses flagged in red, and a risk score. Not legal advice — a comprehension tool.

**Pricing:** $49/month (25 contracts) | $99/month (unlimited) | $9 per-contract one-time

**Revenue math to $5k/month:** 102 at $49 or 51 at $99 or 556 one-time purchases

**Revenue math to $10k/month:** 204 at $49 or 102 at $99

**Sales motion:** SEO content targeting "how to read a vendor contract" and similar intent terms. Free first summary to show the product works. Paid tier unlocks history and bulk use.

**Fulfillment workflow:**
1. User uploads contract PDF
2. Text extracted and chunked
3. Claude API analyzes for key clause categories: obligations, payment, termination, IP, liability, dispute resolution
4. Structured summary generated with risk flags
5. Results displayed and available for download

**AI agent roles:** Clause extraction, category classification, plain-English translation, risk flag identification, summary formatting.

**Human work before stabilization:** 70-90 hours — PDF extraction pipeline, clause classification prompt engineering, output UI, billing, free tier management.

**Human work after stabilization:** 1-2 hours/week — review flagged failures (complex multi-column PDFs and scanned documents break extraction regularly).

**Largest hidden bottleneck:** PDF extraction quality. Contracts come in every format — scanned PDFs, multi-column layouts, handwritten amendments, password-protected files. Getting reliable text extraction across all real-world contract formats takes 3-4 weeks of edge case handling before the product feels solid.

**7-day validation test:** Build a basic demo using Claude API with a contract summary prompt. Share on r/smallbusiness and r/entrepreneur: "I built a tool that summarizes contracts in plain English — try it free." Track usage volume and whether anyone asks for ongoing access.

---

### 5. SOC 2 Evidence Collection Template Pack
**Business quality score: 53.5 / 60**
**Ryan fit score: 11 / 20**

#### Scoring Table

| Criterion | Score | Notes |
|-----------|-------|-------|
| S1 Speed to first dollar | 5 | Post on r/sysadmin, Hacker News, or sell directly on Gumroad; immediate |
| S2 Automation potential (×1.5) | 5 | Digital product; delivery is automated; no ongoing work |
| S3 Gross margin (×1.5) | 5 | 100% margin on a file pack |
| S4 Recurring revenue (×1.5) | 2 | Primarily one-time purchase; annual update upsell is possible but small |
| S5 CS burden | 5 | Documents are self-explanatory; no support needed |
| S6 Sales complexity | 5 | Gumroad self-serve; no sales conversation |
| S7 Operational complexity | 5 | Nothing to operate |
| S8 Market urgency | 5 | Startups facing their first SOC 2 audit are in a panic and actively spending |
| S9 Competitive intensity | 3 | Drata, Vanta bundle this but cost $15k+; template packs in the $300-500 range are open |
| S10 Sub-5-hours/week (×1.5) | 5 | Zero ongoing work after initial build |

**Weighted score:** (5+5+5+5+5+3) + 1.5×(5+5+2+5) = 28 + 25.5 = **53.5**

#### Ryan Fit Table

| Fit Criterion | Score | Notes |
|--------------|-------|-------|
| F1 Market legibility | 2 | SOC 2 compliance is a specialized domain; 30 days is not enough to produce authoritative content |
| F2 Transferable skills | 3 | Technical ops background helps understand the material, but compliance expertise is required for credibility |
| F3 Distribution advantage | 1 | No access to startup CTOs, CISOs, or compliance teams |
| F4 Distraction risk | 5 | Completely separate; no overlap |

**Ryan fit: 11 / 20**

**Customer:** Engineering teams and operations managers at seed-to-Series B startups preparing for their first SOC 2 Type II audit. Typical timeline pressure: customer is requiring SOC 2 before signing.

**Painful problem:** A SOC 2 audit requires assembling evidence across 60-100 controls. Most startups have no idea what evidence to collect, in what format, or how to map it to the Trust Services Criteria. They're either paying $15k+ for compliance software or spending 200+ hours building spreadsheets from scratch.

**Offer:** A complete, auditor-tested evidence collection system: policy templates for all five Trust Services Criteria, evidence collection spreadsheets pre-mapped to each control, audit interview prep guide, gap assessment worksheet, and annotated example evidence. Delivered as a Google Drive folder or Notion template.

**Pricing:** $497 one-time (basic) | $797 (includes annual update access for 2 years)

**Revenue math to $5k/month:** 10 sales at $497 per month

**Revenue math to $10k/month:** 20 sales at $497 per month

**Sales motion:** Search-intent SEO targeting "SOC 2 evidence collection template," "SOC 2 audit preparation checklist." Referral from compliance consultants who recommend it to clients. Hacker News Show HN post.

**Fulfillment workflow:**
1. Customer purchases via Gumroad or Lemon Squeezy
2. Automated delivery of Google Drive link or Notion template
3. Welcome email with setup instructions
4. Nothing else required

**AI agent roles:** Annual content update generation (refresh policies for new AICPA guidance), email follow-up sequences for renewal upsell.

**Human work before stabilization:** 120-160 hours — this requires genuine domain research. The templates must be accurate enough to survive an auditor's review. Cannot be generated without deep understanding of SOC 2 Trust Services Criteria.

**Human work after stabilization:** 2-3 hours/year — update templates when AICPA updates standards.

**Largest hidden bottleneck:** Domain expertise. This is the only top-10 idea where the founder must have or acquire deep subject matter credibility before the product is worth selling. Inaccurate SOC 2 templates cause real damage to startups that rely on them. Ryan would need either 80 hours of research or a content partner with SOC 2 audit experience. That prerequisite is real and takes more than 30 days to satisfy.

**7-day validation test:** Post in r/sysadmin and r/netsec: "Thinking of building a SOC 2 evidence collection template pack for $297 — is this something you'd pay for?" Track replies and ask what's most painful about the current prep process. Also search Gumroad and Podia for existing products to verify pricing assumptions.

---

### 6. AI-Powered Employee Handbook Generator
**Business quality score: 52.5 / 60**
**Ryan fit score: 15 / 20**

#### Scoring Table

| Criterion | Score | Notes |
|-----------|-------|-------|
| S1 Speed to first dollar | 5 | Sell immediately — no infrastructure needed to deliver a generated document |
| S2 Automation potential (×1.5) | 5 | AI generates full handbook from intake form inputs; no human writing required |
| S3 Gross margin (×1.5) | 5 | Software-generated document; near-zero marginal cost |
| S4 Recurring revenue (×1.5) | 2 | Primarily one-time purchase; annual update upsell is real but limited |
| S5 CS burden | 4 | Customers occasionally ask about specific state requirements |
| S6 Sales complexity | 5 | Self-serve intake and checkout; no sales call |
| S7 Operational complexity | 5 | Intake form + AI generation + delivery; simple pipeline |
| S8 Market urgency | 5 | Every business that hires a first employee needs this immediately; urgency is high |
| S9 Competitive intensity | 3 | Zenefits and Gusto bundle this; standalone purchase market is open |
| S10 Sub-5-hours/week (×1.5) | 5 | Fully automated after launch |

**Weighted score:** (5+4+5+5+5+3) + 1.5×(5+5+2+5) = 27 + 25.5 = **52.5**

#### Ryan Fit Table

| Fit Criterion | Score | Notes |
|--------------|-------|-------|
| F1 Market legibility | 4 | Employment law at the surface level required for this product is learnable in 2 weeks |
| F2 Transferable skills | 4 | AI pipeline, technical ops, writing, and SMB sales all directly applicable |
| F3 Distribution advantage | 3 | Contractor and trades business owners are employers; partial distribution overlap |
| F4 Distraction risk | 4 | Does not compete with or distract from current businesses |

**Ryan fit: 15 / 20**

**Customer:** Small business owners hiring their first or first several employees — especially in trades, retail, restaurants, and professional services — who need a compliant employee handbook and cannot afford $500+ in legal fees.

**Painful problem:** Employment lawsuits are expensive. A clear, state-compliant employee handbook is the primary legal protection for small businesses in wrongful termination and discrimination claims. Most small business owners either skip it (legal exposure) or pay a lawyer $1,000+ to write one (expensive).

**Offer:** Answer a 15-question intake form (business type, state, number of employees, policies you want to include). Receive a state-aware, AI-generated employee handbook ready for legal review within 5 minutes. Covers: at-will employment, PTO, conduct standards, harassment policy, and 20 other standard sections.

**Pricing:** $297 one-time (generate + download) | $497 (generate + annual update when state laws change)

**Revenue math to $5k/month:** 17 purchases at $297 per month

**Revenue math to $10k/month:** 34 purchases at $297 per month

**Sales motion:** SEO targeting "employee handbook template" + state modifier (e.g., "California employee handbook template"). This keyword has strong commercial intent and the top results are weak. Affiliate partnership with accountants, HR consultants, and attorneys who serve small businesses.

**Fulfillment workflow:**
1. Customer fills out intake form (business type, state, size, policy preferences)
2. Inputs fed to Claude API with state-specific handbook generation prompt
3. Document generated, formatted as a Google Doc or editable Word file
4. Delivered via email with download link
5. Receipt and disclaimer ("not legal advice") sent automatically

**AI agent roles:** Full handbook generation from intake, state law integration (which requires a maintained state law database), formatting, annual update generation for renewal customers.

**Human work before stabilization:** 80-100 hours — intake form, state law research for 50 states (or the top 10 business-population states to start), prompt engineering, output formatting, billing, delivery automation.

**Human work after stabilization:** 2-3 hours/month — update state law database when employment laws change, monitor for generation failures.

**Largest hidden bottleneck:** State law accuracy. Employment law varies significantly by state. A handbook that misrepresents California's mandatory sick leave policy or New York's harassment training requirements creates legal exposure for the customer — and potentially for the product creator. The state law database must be maintained actively as laws change. Underestimating this ongoing research cost is the most common mistake for this type of product.

**7-day validation test:** Build a basic demo using Claude that generates a handbook from a 5-question intake for one state (Texas). Post on r/smallbusiness: "I built a tool that generates an employee handbook for your state in 5 minutes — try it free." Track usage volume and whether users try to pay for a full version.

---

### 7. Government Contract Award Monitor
**Business quality score: 52 / 60**
**Ryan fit score: 13 / 20**

#### Scoring Table

| Criterion | Score | Notes |
|-----------|-------|-------|
| S1 Speed to first dollar | 3 | Need to find GovCon professionals; cold outreach takes 2-3 weeks |
| S2 Automation potential (×1.5) | 5 | USASpending.gov API + SAM.gov API; fully automated data pipeline |
| S3 Gross margin (×1.5) | 5 | API data + report delivery; near-zero marginal cost |
| S4 Recurring revenue (×1.5) | 5 | Monthly monitoring; award landscape changes constantly |
| S5 CS burden | 4 | Alerts are self-explanatory; minimal support |
| S6 Sales complexity | 3 | GovCon professionals are reachable but not self-serve; short email campaign required |
| S7 Operational complexity | 4 | API integration is real work upfront; low ongoing complexity |
| S8 Market urgency | 5 | Losing a contract to a competitor you didn't know was bidding is deeply painful |
| S9 Competitive intensity | 3 | GovWin and Bloomberg Government compete at $5k-20k/year; sub-$500/month is open |
| S10 Sub-5-hours/week (×1.5) | 5 | Fully automated after setup |

**Weighted score:** (3+4+3+4+5+3) + 1.5×(5+5+5+5) = 22 + 30 = **52**

#### Ryan Fit Table

| Fit Criterion | Score | Notes |
|--------------|-------|-------|
| F1 Market legibility | 3 | GovCon is a specialized world with specific vocabulary; learnable but not fast |
| F2 Transferable skills | 3 | Data pipeline and technical ops apply; no GovCon expertise |
| F3 Distribution advantage | 2 | No existing GovCon relationships |
| F4 Distraction risk | 5 | Completely separate from current businesses |

**Ryan fit: 13 / 20**

**Customer:** Small and mid-size businesses that bid on federal, state, or local government contracts — including defense subcontractors, IT services firms, facilities management companies, and professional services firms in the $1M-50M revenue range.

**Painful problem:** Knowing when a competitor wins a contract — and at what price — is critical intelligence for improving bid strategy. Currently this data is public but requires manual searches across multiple government databases. Most small GovCon firms check manually when they remember to, which is rarely.

**Offer:** Weekly automated report for a specified set of NAICS codes and geographic regions. Shows all new contract awards, winning vendors, contract values, and comparison to previous awards in the same category. Delivered via email every Monday.

**Pricing:** $197/month (one agency/region) | $397/month (multi-region or multiple NAICS codes)

**Revenue math to $5k/month:** 26 single subscribers or 13 multi-region subscribers

**Revenue math to $10k/month:** 51 single or 26 multi-region subscribers

**Sales motion:** Cold email to GovCon professionals (findable via LinkedIn by title + "government contracts"). Lead with a sample report showing their actual NAICS code data. No call required for $197 tier.

**Fulfillment workflow:**
1. Customer selects NAICS codes and state/region preferences during onboarding
2. Automated weekly pull from USASpending.gov API and SAM.gov
3. Data filtered, formatted, and analyzed for notable awards and trends
4. AI generates the "so what" summary for each notable award
5. Email report sent every Monday morning

**AI agent roles:** Data filtering and anomaly detection, award significance scoring, trend identification, natural-language award summaries, competitor pattern analysis.

**Human work before stabilization:** 80-100 hours — API integration, report template design, onboarding flow, billing, state/region preference management.

**Human work after stabilization:** 1-2 hours/week — monitor for API changes, review flagged data quality issues.

**Largest hidden bottleneck:** Data quality. Government contract data is notoriously inconsistent — agency names vary, NAICS codes are self-reported and sometimes wrong, award amounts are amended post-publication. Building a pipeline that produces reliable, trustworthy reports requires significant data cleaning logic that is not visible in the API documentation.

**7-day validation test:** Pull one week of contract award data from USASpending.gov for two NAICS codes (e.g., IT services and facilities management). Format as a simple table. Email it to 10 GovCon professionals on LinkedIn with the subject "I built a free weekly award monitor for your NAICS codes — want the report?" Track reply rate and interest.

---

### 8. Automated Review Request Service (E-Commerce)
**Business quality score: 52 / 60**
**Ryan fit score: 14 / 20**

#### Scoring Table

| Criterion | Score | Notes |
|-----------|-------|-------|
| S1 Speed to first dollar | 4 | E-commerce store owners are reachable; first client possible within a week |
| S2 Automation potential (×1.5) | 5 | Automated email/SMS sequences; zero ongoing human work per client |
| S3 Gross margin (×1.5) | 5 | SaaS delivery; near-zero marginal cost |
| S4 Recurring revenue (×1.5) | 5 | Monthly subscription; churn is low when results are visible |
| S5 CS burden | 4 | Occasional questions about review counts and bounce rates |
| S6 Sales complexity | 4 | Self-serve onboarding possible; short email outreach works |
| S7 Operational complexity | 4 | Email/SMS platform integration requires setup per store; mostly automated |
| S8 Market urgency | 4 | Reviews directly affect conversion rates and ad costs; owners feel this |
| S9 Competitive intensity | 2 | Yotpo, Klaviyo, and Trustpilot all compete; differentiation required |
| S10 Sub-5-hours/week (×1.5) | 5 | Fully automated per-client |

**Weighted score:** (4+4+4+4+4+2) + 1.5×(5+5+5+5) = 22 + 30 = **52**

#### Ryan Fit Table

| Fit Criterion | Score | Notes |
|--------------|-------|-------|
| F1 Market legibility | 4 | Review management is familiar territory from local SEO work |
| F2 Transferable skills | 4 | Email/SMS automation, AI-generated copy, and SMB sales all apply |
| F3 Distribution advantage | 2 | E-commerce is not Ryan's primary world; Skid Steer Nation is a partial entry point |
| F4 Distraction risk | 4 | Does not conflict with current businesses |

**Ryan fit: 14 / 20**

**Customer:** Direct-to-consumer e-commerce store owners on Shopify or WooCommerce with 50-500 orders per month who want more reviews on Google, Trustpilot, or their platform.

**Painful problem:** Reviews drive purchase conversion and reduce Google Ads cost per click. Most store owners know this but have no automated system — they send manual thank-you emails that don't ask for reviews, or they use their email platform's generic automation that has low review conversion rates.

**Offer:** Automated post-purchase review request sequence: SMS at day 3, email at day 5, follow-up email at day 10 for non-responders. Requests routed to the platform with the fewest reviews (Google first, then Trustpilot or platform reviews). Monthly report showing new reviews, star rating trend, and estimated conversion impact.

**Pricing:** $97/month (up to 500 orders/month) | $197/month (up to 2,000 orders/month)

**Revenue math to $5k/month:** 52 at $97 or 26 at $197

**Revenue math to $10k/month:** 103 at $97 or 51 at $197

**Sales motion:** Cold email to Shopify store owners (findable via Shopify store directories). Lead with a benchmark: "The average Shopify store has 12 reviews. Stores with 50+ reviews convert 18% better. Here's how to close that gap automatically." No call required for basic tier.

**Fulfillment workflow:**
1. Store owner connects their e-commerce platform via API or Zapier
2. Order trigger fires post-purchase
3. AI selects review platform with lowest current review count for that customer
4. SMS sent at day 3 (via Twilio), email at day 5, follow-up at day 10
5. Monthly report generated and emailed automatically

**AI agent roles:** Review platform selection per customer, message personalization, negative review detection and interception (direct to private feedback instead of public platform), monthly report generation.

**Human work before stabilization:** 80-100 hours — platform integrations, messaging sequences, billing, reporting pipeline, onboarding flow.

**Human work after stabilization:** 1-2 hours/week — monitor bounce rates, handle Shopify API changes, review flagged negative intercepts.

**Largest hidden bottleneck:** Platform integration fragility. Shopify, WooCommerce, BigCommerce, and Squarespace all have different API structures and webhook behaviors. An integration that works for Shopify breaks on WooCommerce. Starting with one platform is the only way to avoid building three integrations simultaneously — but that limits the addressable market until each integration is built.

**7-day validation test:** Reach out to 10 Shopify store owners in a Facebook group or via LinkedIn. Ask: "Do you have an automated system for collecting post-purchase reviews? If not, what's stopping you?" Track the response and identify what objection or gap they name. Secondary test: check Shopify App Store reviews of existing review apps to understand what users complain about — that is your differentiation angle.

---

### 9. SaaS Tool Replacement Finder
**Business quality score: 50.5 / 60**
**Ryan fit score: 15 / 20**

#### Scoring Table

| Criterion | Score | Notes |
|-----------|-------|-------|
| S1 Speed to first dollar | 4 | Free tool drives traffic; affiliate commissions begin immediately on referrals |
| S2 Automation potential (×1.5) | 4 | AI generates recommendations; affiliate link insertion is automated; some prompt tuning needed |
| S3 Gross margin (×1.5) | 5 | Affiliate model; 100% margin on referral fees |
| S4 Recurring revenue (×1.5) | 3 | Affiliate commissions are one-time per referral; some tools pay monthly recurring |
| S5 CS burden | 5 | Free tool; no client relationship |
| S6 Sales complexity | 5 | Free tool; no sales conversation |
| S7 Operational complexity | 4 | Once built, low maintenance; affiliate programs occasionally change terms |
| S8 Market urgency | 4 | SaaS budget pressure is real; companies actively looking to cut costs |
| S9 Competitive intensity | 3 | AlternativeTo.net, G2 alternatives pages exist; intelligent recommendation angle is less crowded |
| S10 Sub-5-hours/week (×1.5) | 5 | Fully automated; only affiliate program management requires occasional attention |

**Weighted score:** (4+5+5+4+4+3) + 1.5×(4+5+3+5) = 25 + 25.5 = **50.5**

#### Ryan Fit Table

| Fit Criterion | Score | Notes |
|--------------|-------|-------|
| F1 Market legibility | 4 | Ryan uses SaaS tools daily; understands the buyer's problem from personal experience |
| F2 Transferable skills | 4 | AI pipeline, technical ops, and writing all apply directly |
| F3 Distribution advantage | 3 | Can reach agency and SMB audience through existing contacts |
| F4 Distraction risk | 4 | No conflict with current businesses |

**Ryan fit: 15 / 20**

**Customer:** Operations managers, founders, and IT leads at companies with $50k-500k annual SaaS spend who are under pressure to cut software costs or find better tools for their stack.

**Painful problem:** Finding a cheaper or better alternative to a specific SaaS tool requires hours of research across G2, Capterra, and Reddit. The comparison is never apples-to-apples and pricing pages are deliberately opaque.

**Offer:** Enter your current tool and budget. Receive a ranked list of alternatives with: feature comparison, real pricing (not "contact sales"), integration compatibility check, and estimated migration effort. Results in 30 seconds.

**Pricing:** Free to use. Revenue from affiliate commissions (typically $50-$500 per referred signup, plus recurring commissions from tools that offer revenue share).

**Revenue math to $5k/month:** Depends on mix; a tool averaging $200 commission requires 25 conversions/month

**Revenue math to $10k/month:** 50 conversions/month at $200 average or 20 at $500

**Sales motion:** Free tool with strong SEO targeting "[tool name] alternative" keywords (e.g., "Slack alternative," "HubSpot alternative"). These keywords have high commercial intent and clear monetization through affiliate programs. No outbound required.

**Fulfillment workflow:**
1. User enters current tool name and context (team size, budget, key features needed)
2. Claude API queries a maintained database of alternatives + affiliate program data
3. Ranked recommendations generated with feature comparison and pricing
4. Affiliate links inserted automatically for each recommended tool
5. User clicks through to tool; affiliate commission tracked via referral links

**AI agent roles:** Alternative matching, feature comparison generation, pricing normalization, recommendation ranking, new tool database additions (monitoring Product Hunt and SaaS directories).

**Human work before stabilization:** 100-120 hours — build initial tool database (500+ tools with affiliate programs, pricing, features), prompt engineering for recommendation quality, affiliate program signup and link management, SEO content for major tool categories.

**Human work after stabilization:** 2-3 hours/week — add new tools to database, monitor affiliate program changes, update pricing as tools change their plans.

**Largest hidden bottleneck:** Affiliate program scale. The economics only work if you have affiliate relationships with enough tools that the recommendation engine always has a monetizable option. Many good alternative tools don't have affiliate programs, which means recommending them earns nothing. Building a database where the best recommendations are also the most monetizable requires careful curation and potentially paying for access to tool data.

**7-day validation test:** Build a single-page tool using Claude API that accepts a tool name and returns 3 alternatives with pricing. Test it against 10 popular tools. Post on r/SaaS and r/entrepreneur. Track clicks on the alternatives listed and ask users whether they'd want this for their full stack.

---

### 10. Permit Expiration Alert Service
**Business quality score: 50 / 60**
**Ryan fit score: 13 / 20**

#### Scoring Table

| Criterion | Score | Notes |
|-----------|-------|-------|
| S1 Speed to first dollar | 3 | Finding property managers requires targeted outreach; 2-3 weeks to first client |
| S2 Automation potential (×1.5) | 4 | Automated monitoring with some data-source variability |
| S3 Gross margin (×1.5) | 5 | Software delivery; near-zero marginal cost |
| S4 Recurring revenue (×1.5) | 5 | Monthly monitoring; permits expire on a rolling basis |
| S5 CS burden | 5 | Alerts are self-explanatory; property managers act on them without support |
| S6 Sales complexity | 3 | Property managers are reachable but not self-serve; direct outreach required |
| S7 Operational complexity | 3 | Municipal data sources are inconsistent; coverage gaps require ongoing work |
| S8 Market urgency | 5 | Expired permits cause certificate of occupancy failures, tenant complaints, and fines |
| S9 Competitive intensity | 4 | Very few direct competitors at this price point |
| S10 Sub-5-hours/week (×1.5) | 4 | Mostly automated; occasional source maintenance |

**Weighted score:** (3+5+3+3+5+4) + 1.5×(4+5+5+4) = 23 + 27 = **50**

#### Ryan Fit Table

| Fit Criterion | Score | Notes |
|--------------|-------|-------|
| F1 Market legibility | 3 | Commercial property management is not Ryan's domain; learnable but not fast |
| F2 Transferable skills | 3 | Data pipeline and technical ops apply; property management knowledge does not |
| F3 Distribution advantage | 2 | No commercial property manager relationships |
| F4 Distraction risk | 5 | Completely separate; no overlap |

**Ryan fit: 13 / 20**

**Customer:** Commercial property managers and portfolio owners responsible for 10-100 commercial properties — office parks, retail centers, industrial buildings — where multiple permits (elevator, fire suppression, boiler, HVAC, electrical) must be maintained.

**Painful problem:** A single expired permit discovered during a city inspection can halt tenant operations, trigger fines, and invalidate insurance claims. Property managers track permit expiration manually or not at all, relying on vendor calls that don't always come.

**Offer:** Monthly monitoring of all active permits for a commercial property portfolio. Automated alerts at 90, 60, and 30 days before expiration. Monthly status report listing all upcoming expirations, responsible party, and renewal instructions.

**Pricing:** $97/month (up to 10 properties) | $197/month (up to 50 properties)

**Revenue math to $5k/month:** 52 at $97 or 26 at $197

**Revenue math to $10k/month:** 103 at $97 or 51 at $197

**Sales motion:** Cold email to commercial property management companies (findable via LinkedIn and IREM member directories). Lead with one specific permit type as the hook: "Is your elevator permit current? Here's a free check for your portfolio."

**Fulfillment workflow:**
1. Client provides property addresses at onboarding
2. System queries municipal permit databases for each property
3. Permit expiration dates logged and scheduled for alerts
4. Automated alert emails at 90/60/30-day thresholds
5. Monthly summary report generated and emailed

**AI agent roles:** Permit data parsing from varied municipal formats, alert email personalization, renewal instruction generation by permit type and jurisdiction.

**Human work before stabilization:** 100-120 hours — municipal database research and integration (each city has a different portal), permit type taxonomy, alert system, onboarding.

**Human work after stabilization:** 3-4 hours/week — municipal database sources change more often than expected; new client onboarding requires verifying coverage for their specific city.

**Largest hidden bottleneck:** Municipal data access. Permit data is not uniformly accessible via API. Many cities use legacy systems with no API — data must be scraped or manually checked. Coverage gaps mean you cannot confidently serve clients in cities where data is unavailable, which limits the addressable market and requires geographic rollout planning.

**7-day validation test:** Check whether 5 major US cities (New York, Los Angeles, Chicago, Houston, Phoenix) have accessible permit databases with expiration dates. If 3 of 5 do, the data foundation exists. Then cold email 5 commercial property managers and offer a free portfolio audit for one property type.

---

## Ideas 11–30 — Scored Table Only

| Rank | Idea | Category | Weighted Score | Key weakness |
|------|------|----------|---------------|--------------|
| 11 | Price Tracking & Competitive Intel (E-Commerce) | Data monitoring | 50 | Competition from Prisync, DataHen; S9=2 |
| 12 | Financial Model Template Library | Digital product | 49.5 | Low recurring (S4=2); one-time purchases |
| 13 | AI Prompt Library Subscription | Digital product | 49.5 | Extremely crowded market; S9=1 |
| 14 | Regulatory Change Digest (SaaS Compliance) | B2B info product | 49 | Finding subscribers is slow; S1=3 |
| 15 | OSHA Compliance Document Generator | Compliance service | 48.5 | Low recurring (S4=2); one-time purchase model |
| 16 | Job Posting Trend Monitor | Data monitoring | 47.5 | Burning Glass, LinkedIn compete; S9=2 |
| 17 | AI-Powered RFP Response Generator | Software service | 46.5 | Loopio, Responsive compete; setup per client |
| 18 | B2B Benchmark Reports by Role | B2B info product | 46.5 | Data collection is hard to automate; S2=4 |
| 19 | AI Agent Prompt Framework License | Licensing | 45.5 | Early market; S8=3; hard to sell without case studies |
| 20 | Commercial RE Permit & Zoning Feed | Data monitoring | 45.5 | CoStar, BuildZoom compete; data cleaning ongoing |
| 21 | Competitive Landscape Reports for VCs | Productized research | 44 | Warm intro required to reach VCs; S6=3 |
| 22 | Independent Insurance Agency Finder | Niche directory | 44 | Data verification is ongoing work; EverQuote competes |
| 23 | Verified Franchise Opportunity Directory | Niche directory | 43 | Build time before launch; FranchiseGator competes |
| 24 | Verified M&A Advisor Directory | Niche directory | 42.5 | Build time before launch; Axial competes |
| 25 | White-Label AI Report Generator | Licensing | 42 | Agency customers are demanding; S5=3, S7=3 |
| 26 | Niche Industry Salary Benchmarking | B2B info product | 41 | Data collection is hard; Radford, Levels.fyi compete |
| 27 | Market Entry Analysis for B2B SaaS | Productized research | 40 | Low recurring; AI quality requires human review |
| 28 | B2B Software Vendor Comparison | Marketplace | 39 | G2, Capterra dominate; cold-start problem; S9=1 |
| 29 | Verified Expert Marketplace | Marketplace | 36 | Two-sided cold start; quality control is human work |
| 30 | Micro-Consulting Marketplace | Marketplace | 29 | Clarity.fm competes; two-sided cold start; S7=1 |
