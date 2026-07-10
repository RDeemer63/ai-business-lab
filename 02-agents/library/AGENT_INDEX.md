# Agent Library Index

**Source:** https://github.com/msitarzewski/agency-agents (MIT License)
**Imported:** 2026-07-09
**License file:** `vendor-licenses/agency-agents-LICENSE`

---

## Summary

| Metric | Count |
|--------|-------|
| Total files imported | 276 |
| Pure agent files (with frontmatter) | 243 |
| Framework/playbook documents | 13 (strategy/) |
| Example workflow documents | 5 (examples/) |
| Integration examples | 1 (integrations/) |
| Departments covered | 18 |

| Relevance to AI Business Lab | Count |
|------------------------------|-------|
| High | 31 |
| Medium | 52 |
| Low | 160 |

| Department | Agent Count | High | Medium | Low |
|------------|-------------|------|--------|-----|
| Academic | 6 | 0 | 1 | 5 |
| Design | 9 | 0 | 4 | 5 |
| Engineering | 49 | 7 | 14 | 28 |
| Finance | 5 | 3 | 2 | 0 |
| Game Development | 19 | 0 | 0 | 19 |
| GIS | 13 | 0 | 0 | 13 |
| Healthcare | 3 | 0 | 0 | 3 |
| Integrations | 1 | 0 | 1 | 0 |
| Marketing | 35 | 10 | 10 | 15 |
| Paid Media | 7 | 3 | 3 | 1 |
| Product | 5 | 3 | 2 | 0 |
| Project Management | 7 | 2 | 4 | 1 |
| Sales | 9 | 7 | 2 | 0 |
| Security | 10 | 0 | 3 | 7 |
| Spatial Computing | 6 | 0 | 0 | 6 |
| Specialized | 44 | 8 | 15 | 21 |
| Support | 6 | 3 | 2 | 1 |
| Testing | 9 | 0 | 4 | 5 |

---

## Overlap / Duplicate Flags

| Library Agent | Our Custom Agent | Overlap Type |
|---------------|-----------------|--------------|
| `specialized/specialized-chief-of-staff.md` | `custom/chief-of-staff.md` | Direct duplicate — same role. Our version is more specific to AI Business Lab operations. |
| `product/product-trend-researcher.md` | `custom/business-research.md` | Partial — trend research is a subset of business research. Keep both; different scope. |
| `marketing/marketing-content-creator.md` | `custom/newsletter-editor.md` | Partial — content creator is broader; newsletter editor is narrow and voice-specific. Keep both. |
| `specialized/business-strategist.md` | `custom/chief-of-staff.md` | Partial — CoS handles coordination; Business Strategist handles analysis. Complementary, not duplicate. |
| `sales/sales-outreach.md` | `specialized/sales-outreach.md` | Duplicate file under different paths — different agent but same name. Compare before activating either. |

---

## Marketing Department

### SEO Specialist
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-seo-specialist.md`
- **Department:** Marketing
- **Primary purpose:** Technical SEO, content optimization, link building, and local search strategy.
- **Expected inputs:** Site URL, target keywords, competitor list, Search Console access.
- **Expected outputs:** Technical audit, keyword strategy, on-page checklist, link building plan, monthly report.
- **Likely tools required:** WebFetch, WebSearch, Read, Write, Edit
- **Relevance to AI Business Lab:** HIGH — directly relevant to the AI local SEO subscription product (Finalist 2) and to Throttled Up Platform's core delivery.

### Email Marketing Strategist
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-email-strategist.md`
- **Department:** Marketing
- **Primary purpose:** CRM-driven email campaigns, lifecycle automation, segmentation, and deliverability.
- **Expected inputs:** Audience segments, product offer, campaign goal, current email performance data.
- **Expected outputs:** Email sequences, segmentation architecture, A/B test plan, deliverability checklist.
- **Likely tools required:** WebFetch, WebSearch, Write, Edit
- **Relevance to AI Business Lab:** HIGH — needed for client nurture sequences and AI Business Lab's own lead pipeline.

### Content Creator
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-content-creator.md`
- **Department:** Marketing
- **Primary purpose:** Multi-platform content strategy, editorial calendars, and brand storytelling.
- **Expected inputs:** Brand brief, target audience, content goals, channel list.
- **Expected outputs:** Editorial calendar, content drafts, repurposing plan.
- **Likely tools required:** WebFetch, WebSearch, Read, Write, Edit
- **Relevance to AI Business Lab:** HIGH — core to the AI content subscription product (Finalist 1). Partial overlap with Newsletter Editor (our custom agent); Newsletter Editor is voice-specific, this is broader.

### Growth Hacker
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-growth-hacker.md`
- **Department:** Marketing
- **Primary purpose:** Rapid user acquisition through viral loops, funnel optimization, and growth experiments.
- **Expected inputs:** Product, current conversion data, target customer segment, budget.
- **Expected outputs:** Growth experiment backlog, funnel analysis, channel recommendations, viral loop design.
- **Likely tools required:** WebFetch, WebSearch, Read, Write, Edit
- **Relevance to AI Business Lab:** HIGH — Phase 1 validation requires fast client acquisition experiments.

### PR & Communications Manager
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-pr-communications-manager.md`
- **Department:** Marketing
- **Primary purpose:** Media relations, press releases, crisis communications, and brand reputation management.
- **Expected inputs:** Story angle, brand positioning, target publications, spokesperson bio.
- **Expected outputs:** Press release, media pitch, messaging framework, stakeholder communications.
- **Likely tools required:** WebFetch, WebSearch, Write, Edit
- **Relevance to AI Business Lab:** HIGH — useful for OTW book PR and AI Business Lab public positioning as the experiment gains traction.

### Social Media Strategist
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-social-media-strategist.md`
- **Department:** Marketing
- **Primary purpose:** Cross-platform social strategy, community management, and thought leadership for LinkedIn and Twitter.
- **Expected inputs:** Brand voice, target audience, content pillars, posting cadence.
- **Expected outputs:** Social calendar, post drafts, engagement strategy, analytics framework.
- **Likely tools required:** WebFetch, WebSearch, Read, Write, Edit
- **Relevance to AI Business Lab:** HIGH — supports the newsletter and contractor audience building.

### Video Optimization Specialist
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-video-optimization-specialist.md`
- **Department:** Marketing
- **Primary purpose:** YouTube algorithm optimization, thumbnail strategy, chaptering, and cross-platform video syndication.
- **Expected inputs:** Video content, target keywords, channel analytics.
- **Expected outputs:** Video SEO recommendations, thumbnail concepts, description templates, channel strategy.
- **Likely tools required:** WebFetch, WebSearch, Write, Edit
- **Relevance to AI Business Lab:** HIGH — directly relevant to the YouTube Script System (Finalist 4).

### LinkedIn Content Creator
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-linkedin-content-creator.md`
- **Department:** Marketing
- **Primary purpose:** LinkedIn thought leadership, personal brand building, and high-engagement professional content.
- **Expected inputs:** Brand voice, expertise topics, audience type, posting frequency.
- **Expected outputs:** LinkedIn post drafts, thread ideas, engagement strategy, profile recommendations.
- **Likely tools required:** WebFetch, WebSearch, Write, Edit
- **Relevance to AI Business Lab:** HIGH — Ryan's LinkedIn presence is a distribution channel for all three businesses.

### Global Podcast Strategist
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-global-podcast-strategist.md`
- **Department:** Marketing
- **Primary purpose:** Podcast positioning, audience development, content strategy, and monetization.
- **Expected inputs:** Show concept, target audience, competitive landscape.
- **Expected outputs:** Show positioning document, episode arc, monetization plan, distribution strategy.
- **Likely tools required:** WebFetch, WebSearch, Write, Edit
- **Relevance to AI Business Lab:** HIGH — relevant to OTW brand building and the newsletter-to-podcast expansion path.

### Book Co-Author
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-book-co-author.md`
- **Department:** Marketing
- **Primary purpose:** Thought leadership book development from voice notes and fragments into structured chapters.
- **Expected inputs:** Voice notes, raw ideas, positioning, target reader.
- **Expected outputs:** Structured chapters, narrative arc, first-person draft.
- **Likely tools required:** Read, Write, Edit
- **Relevance to AI Business Lab:** HIGH — directly relevant to OTW book content development.

### App Store Optimizer
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-app-store-optimizer.md`
- **Department:** Marketing
- **Primary purpose:** App Store Optimization for discoverability and conversion.
- **Expected inputs:** App name, category, competitor apps, current metrics.
- **Expected outputs:** ASO audit, keyword strategy, store listing copy.
- **Likely tools required:** WebFetch, WebSearch, Write
- **Relevance to AI Business Lab:** MEDIUM — relevant if Tulboxx develops a mobile presence.

### AEO Foundations Architect
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-aeo-foundations.md`
- **Department:** Marketing
- **Primary purpose:** AI Engine Optimization — making content visible and citable by AI crawlers.
- **Expected inputs:** Website URL, existing content, target AI platforms.
- **Expected outputs:** llms.txt implementation, structured content plan, AI-visibility audit.
- **Likely tools required:** WebFetch, WebSearch, Write, Edit
- **Relevance to AI Business Lab:** MEDIUM — emerging channel relevant to OTW and Throttled Up positioning.

### Agentic Search Optimizer
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-agentic-search-optimizer.md`
- **Department:** Marketing
- **Primary purpose:** WebMCP readiness — ensuring AI agents can complete tasks on your website.
- **Expected inputs:** Website URL, target task flows.
- **Expected outputs:** WebMCP audit, implementation recommendations.
- **Likely tools required:** WebFetch, WebSearch, Write
- **Relevance to AI Business Lab:** MEDIUM — forward-looking but relevant as AI-native buyers increase.

### AI Citation Strategist
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-ai-citation-strategist.md`
- **Department:** Marketing
- **Primary purpose:** Optimize brand visibility in ChatGPT, Claude, Gemini, and Perplexity recommendations.
- **Expected inputs:** Brand name, competitors, target queries.
- **Expected outputs:** Citation audit, content fixes, authority-building plan.
- **Likely tools required:** WebFetch, WebSearch, Write
- **Relevance to AI Business Lab:** MEDIUM — emerging relevance as AI search grows.

### Twitter/X Engager
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-twitter-engager.md`
- **Department:** Marketing
- **Primary purpose:** Real-time Twitter engagement, thought leadership, and viral thread creation.
- **Expected inputs:** Brand voice, target topics, competitor accounts.
- **Expected outputs:** Thread drafts, engagement targets, content calendar.
- **Likely tools required:** WebFetch, WebSearch, Write
- **Relevance to AI Business Lab:** MEDIUM — supporting channel for public building of this experiment.

### X/Twitter Intelligence Analyst
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-x-twitter-intelligence-analyst.md`
- **Department:** Marketing
- **Primary purpose:** Social intelligence, trend detection, and account monitoring on X.
- **Expected inputs:** Target accounts, keywords, monitoring parameters.
- **Expected outputs:** Trend reports, audience insights, competitive intelligence.
- **Likely tools required:** WebFetch, WebSearch, Write
- **Relevance to AI Business Lab:** MEDIUM — useful for contractor audience research.

### Reddit Community Builder
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-reddit-community-builder.md`
- **Department:** Marketing
- **Primary purpose:** Authentic Reddit community engagement and value-driven content.
- **Expected inputs:** Target subreddits, brand positioning, value proposition.
- **Expected outputs:** Engagement plan, content strategy, community map.
- **Likely tools required:** WebFetch, WebSearch, Write
- **Relevance to AI Business Lab:** MEDIUM — r/Entrepreneur, r/smallbusiness, r/ContractorAdvice are viable channels.

### Instagram Curator
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-instagram-curator.md`
- **Department:** Marketing
- **Primary purpose:** Instagram visual storytelling, community building, and multi-format content.
- **Expected inputs:** Brand aesthetic, target audience, content pillars.
- **Expected outputs:** Content calendar, caption templates, hashtag strategy.
- **Likely tools required:** WebFetch, WebSearch, Write
- **Relevance to AI Business Lab:** MEDIUM — secondary channel; relevant for OTW brand building.

### Carousel Growth Engine
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-carousel-growth-engine.md`
- **Department:** Marketing
- **Primary purpose:** Autonomous TikTok and Instagram carousel generation and publishing.
- **Expected inputs:** Website URL, campaign goal, target platform.
- **Expected outputs:** 6-slide carousel content, auto-publish to feed.
- **Likely tools required:** WebFetch, Playwright, API access
- **Relevance to AI Business Lab:** MEDIUM — automation potential is high if social content is in scope.

### TikTok Strategist
- **Source file:** `02-agents/library/agency-agents/marketing/marketing-tiktok-strategist.md`
- **Department:** Marketing
- **Primary purpose:** TikTok viral content creation, algorithm optimization, and community building.
- **Expected inputs:** Brand voice, target audience, competitor analysis.
- **Expected outputs:** TikTok content plan, video scripts, trend integration.
- **Likely tools required:** WebFetch, WebSearch, Write
- **Relevance to AI Business Lab:** LOW — not a priority platform for the contractor market.

*(Note: China-specific marketing agents — Baidu, Bilibili, Douyin, Kuaishou, WeChat, Weibo, Xiaohongshu, Zhihu, China e-commerce, cross-border e-commerce, private domain, short video editing, multi-platform publisher, podcast strategist [China], livestream commerce, China market localization — are rated LOW as they are outside the target market.)*

---

## Sales Department

### Offer & Lead Gen Strategist
- **Source file:** `02-agents/library/agency-agents/sales/sales-offer-lead-gen-strategist.md`
- **Department:** Sales
- **Primary purpose:** Design irresistible offers and lead magnets that attract qualified buyers at scale.
- **Expected inputs:** Product/service, target customer, unique value proposition, pricing range.
- **Expected outputs:** Offer structure, lead magnet concepts, multi-channel lead gen plan.
- **Likely tools required:** WebFetch, WebSearch, Write, Edit
- **Relevance to AI Business Lab:** HIGH — Phase 1 requires designing and testing the first offer.

### Outbound Strategist
- **Source file:** `02-agents/library/agency-agents/sales/sales-outbound-strategist.md`
- **Department:** Sales
- **Primary purpose:** Signal-based multi-channel prospecting sequences and ICP definition.
- **Expected inputs:** ICP description, product/service, prospecting budget, target volume.
- **Expected outputs:** Prospect list criteria, outreach sequences, personalization framework.
- **Likely tools required:** WebFetch, WebSearch, Write
- **Relevance to AI Business Lab:** HIGH — reaching first clients requires a systematic outbound approach.

### Sales Coach
- **Source file:** `02-agents/library/agency-agents/sales/sales-coach.md`
- **Department:** Sales
- **Primary purpose:** Rep development, pipeline review facilitation, and call coaching.
- **Expected inputs:** Sales call transcripts, deal notes, pipeline stage data.
- **Expected outputs:** Coaching feedback, deal strategy, forecast accuracy improvement.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** HIGH — Ryan is the sole salesperson; a coaching framework for his own calls improves close rate.

### Deal Strategist
- **Source file:** `02-agents/library/agency-agents/sales/sales-deal-strategist.md`
- **Department:** Sales
- **Primary purpose:** MEDDPICC qualification, competitive positioning, and win planning for complex sales cycles.
- **Expected inputs:** Deal details, stakeholder map, competitive landscape.
- **Expected outputs:** Deal scorecard, win plan, competitive response.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** HIGH — useful once first clients are in pipeline at $750-$1,500/month price points.

### Proposal Strategist
- **Source file:** `02-agents/library/agency-agents/sales/sales-proposal-strategist.md`
- **Department:** Sales
- **Primary purpose:** Transform RFPs and opportunities into compelling win narratives.
- **Expected inputs:** RFP or prospect requirements, value proposition, competitive differentiation.
- **Expected outputs:** Proposal document, executive summary, win themes.
- **Likely tools required:** Read, Write, Edit
- **Relevance to AI Business Lab:** HIGH — client proposals for Throttled Up services need to be polished and consistent.

### Sales Outreach
- **Source file:** `02-agents/library/agency-agents/specialized/sales-outreach.md`
- **Department:** Sales
- **Primary purpose:** Consultative B2B cold prospecting, lead follow-up, and objection handling.
- **Expected inputs:** Prospect list, product, value prop, objection list.
- **Expected outputs:** Outreach messages, follow-up sequences, objection responses.
- **Likely tools required:** Write, Edit
- **Relevance to AI Business Lab:** HIGH — complements Outbound Strategist; this executes the outreach.
- **Note:** Also exists at `specialized/sales-outreach.md` — same filename, different path. Review both before activating.

### Account Strategist
- **Source file:** `02-agents/library/agency-agents/sales/sales-account-strategist.md`
- **Department:** Sales
- **Primary purpose:** Land-and-expand execution, QBR facilitation, and net revenue retention.
- **Expected inputs:** Existing account data, expansion goals, stakeholder map.
- **Expected outputs:** Account growth plan, QBR deck, expansion pitch.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** HIGH — retaining and expanding early clients is critical to reaching $10k MRR.

### Discovery Coach
- **Source file:** `02-agents/library/agency-agents/sales/sales-discovery-coach.md`
- **Department:** Sales
- **Primary purpose:** Coaches sales teams on discovery methodology and question design.
- **Expected inputs:** Discovery call structure, common objections, target ICP.
- **Expected outputs:** Discovery question bank, call framework, debrief template.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** MEDIUM — useful once there are consistent sales calls to review.

### Pipeline Analyst
- **Source file:** `02-agents/library/agency-agents/sales/sales-pipeline-analyst.md`
- **Department:** Sales
- **Primary purpose:** Pipeline health diagnostics, deal velocity analysis, and forecast accuracy.
- **Expected inputs:** CRM data, pipeline stage definitions, deal history.
- **Expected outputs:** Pipeline health report, velocity analysis, forecast.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** MEDIUM — relevant at Phase 2 when there are 10+ deals to analyze.

### Sales Engineer
- **Source file:** `02-agents/library/agency-agents/sales/sales-engineer.md`
- **Department:** Sales
- **Primary purpose:** Technical discovery, demo engineering, POC scoping, and competitive battlecards.
- **Expected inputs:** Technical requirements, product capabilities, competitor specs.
- **Expected outputs:** Demo script, technical battlecard, POC scope.
- **Likely tools required:** Read, Write, WebFetch
- **Relevance to AI Business Lab:** LOW — premature until Tulboxx has a formal sales process with technical evaluation stages.

---

## Specialized Department

### Business Strategist
- **Source file:** `02-agents/library/agency-agents/specialized/business-strategist.md`
- **Department:** Strategy
- **Primary purpose:** Competitive analysis, market entry strategy, business model design, and growth planning.
- **Expected inputs:** Market description, competitive landscape, business goals, constraints.
- **Expected outputs:** Market analysis, competitive positioning, strategic options, recommendation.
- **Likely tools required:** WebFetch, WebSearch, Write
- **Relevance to AI Business Lab:** HIGH — directly useful for Phase 1 strategy selection.

### Pricing Analyst
- **Source file:** `02-agents/library/agency-agents/specialized/specialized-pricing-analyst.md`
- **Department:** Strategy
- **Primary purpose:** Develop optimal pricing models through market research and margin analysis.
- **Expected inputs:** Product description, target market, competitor pricing, cost structure.
- **Expected outputs:** Pricing model, tier recommendations, price sensitivity analysis.
- **Likely tools required:** WebFetch, WebSearch, Write, Edit
- **Relevance to AI Business Lab:** HIGH — pricing the first offer correctly is a Phase 1 decision.

### Customer Success Manager
- **Source file:** `02-agents/library/agency-agents/specialized/customer-success-manager.md`
- **Department:** Operations
- **Primary purpose:** Onboarding, health scoring, churn prevention, and renewal management.
- **Expected inputs:** Customer data, onboarding status, product usage signals.
- **Expected outputs:** Onboarding playbook, health scorecard, churn risk flags, expansion plan.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** HIGH — client retention from month 1 is the survival metric.

### Agents Orchestrator
- **Source file:** `02-agents/library/agency-agents/specialized/agents-orchestrator.md`
- **Department:** Engineering / Strategy
- **Primary purpose:** Orchestrates the full development workflow across multiple agents.
- **Expected inputs:** Project brief, agent roster, task list.
- **Expected outputs:** Delegated tasks, coordinated outputs, pipeline status.
- **Likely tools required:** Full tool access
- **Relevance to AI Business Lab:** HIGH — directly applicable to the Chief of Staff orchestration pattern.

### Operations Manager
- **Source file:** `02-agents/library/agency-agents/specialized/operations-manager.md`
- **Department:** Operations
- **Primary purpose:** Process mapping, capacity planning, KPI governance, and organizational efficiency.
- **Expected inputs:** Current processes, bottlenecks, KPIs, org structure.
- **Expected outputs:** Process maps, efficiency recommendations, KPI dashboard design.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** HIGH — as client count grows, operational efficiency becomes critical.

### Chief of Staff (upstream)
- **Source file:** `02-agents/library/agency-agents/specialized/specialized-chief-of-staff.md`
- **Department:** Strategy
- **Primary purpose:** Master coordinator for founders — filters noise, routes decisions, enforces consistency.
- **Expected inputs:** Task list, decisions, stakeholder communications.
- **Expected outputs:** Prioritized actions, routed decisions, cleaned-up outputs.
- **Likely tools required:** Read, Write, Edit
- **Relevance to AI Business Lab:** MEDIUM — overlaps with our custom Chief of Staff. Review for ideas to incorporate; do not activate as separate agent.
- **Overlap:** Duplicate of our `custom/chief-of-staff.md`.

### Executive Summary Generator
- **Source file:** `02-agents/library/agency-agents/support/support-executive-summary-generator.md`
- **Department:** Support
- **Primary purpose:** Transforms complex business inputs into concise executive summaries.
- **Expected inputs:** Research data, meeting notes, analysis output.
- **Expected outputs:** Executive summary document using McKinsey/BCG frameworks.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** HIGH — useful for condensing research into decision briefs (like the TOP5 brief).

### Automation Governance Architect
- **Source file:** `02-agents/library/agency-agents/specialized/automation-governance-architect.md`
- **Department:** Operations
- **Primary purpose:** Audits value, risk, and maintainability of business automations before building.
- **Expected inputs:** Automation concept, current tools, risk tolerance.
- **Expected outputs:** Build/no-build recommendation, risk assessment, governance framework.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** MEDIUM — relevant before building GHL automation systems.

### Workflow Architect
- **Source file:** `02-agents/library/agency-agents/specialized/specialized-workflow-architect.md`
- **Department:** Operations
- **Primary purpose:** Maps complete workflow trees including failure modes, handoff contracts, and recovery paths.
- **Expected inputs:** System description, user journey, agent interactions.
- **Expected outputs:** Workflow map, build-ready spec, QA test cases.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** MEDIUM — valuable for documenting the AI delivery pipeline before building.

### Customer Service
- **Source file:** `02-agents/library/agency-agents/specialized/customer-service.md`
- **Department:** Operations
- **Primary purpose:** Handles inquiries, complaints, account support, and escalation.
- **Expected inputs:** Customer message, product context, issue type.
- **Expected outputs:** Response, resolution, escalation flag.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** MEDIUM — relevant for handling client inquiries once volume grows.

### MCP Builder
- **Source file:** `02-agents/library/agency-agents/specialized/specialized-mcp-builder.md`
- **Department:** Engineering
- **Primary purpose:** Designs, builds, and tests MCP servers that extend AI agent capabilities.
- **Expected inputs:** Tool requirements, API specs, agent workflow.
- **Expected outputs:** Working MCP server, documentation, test suite.
- **Likely tools required:** Bash, Read, Write, Edit
- **Relevance to AI Business Lab:** MEDIUM — relevant for extending the AI-OS agent system.

*(Remaining specialized agents — legal, healthcare, finance-specific, cultural/market-specific, government, blockchain, and other niche roles — are rated LOW for Phase 1 relevance.)*

---

## Finance Department

### Financial Analyst
- **Source file:** `02-agents/library/agency-agents/finance/finance-financial-analyst.md`
- **Department:** Finance
- **Primary purpose:** Financial modeling, forecasting, scenario analysis, and decision support.
- **Expected inputs:** Revenue data, cost structure, growth assumptions.
- **Expected outputs:** Financial model, forecast, scenario analysis.
- **Likely tools required:** Read, Write, Edit
- **Relevance to AI Business Lab:** HIGH — building the MRR model and tracking revenue path to $10k.

### FP&A Analyst
- **Source file:** `02-agents/library/agency-agents/finance/finance-fpa-analyst.md`
- **Department:** Finance
- **Primary purpose:** Budgeting, variance analysis, and strategic resource allocation.
- **Expected inputs:** Budget, actuals, strategic priorities.
- **Expected outputs:** Budget plan, variance report, resource allocation recommendation.
- **Likely tools required:** Read, Write, Edit
- **Relevance to AI Business Lab:** HIGH — managing spend discipline as the business invests in tools and infrastructure.

### Bookkeeper & Controller
- **Source file:** `02-agents/library/agency-agents/finance/finance-bookkeeper-controller.md`
- **Department:** Finance
- **Primary purpose:** Day-to-day accounting, financial reconciliations, and month-end close.
- **Expected inputs:** Transaction data, accounts, reporting period.
- **Expected outputs:** Reconciliation, financial statements, close checklist.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** HIGH — as revenue comes in, clean books are required.

### Tax Strategist
- **Source file:** `02-agents/library/agency-agents/finance/finance-tax-strategist.md`
- **Department:** Finance
- **Primary purpose:** Tax optimization and multi-jurisdictional compliance.
- **Expected inputs:** Business structure, revenue, expenses, jurisdiction.
- **Expected outputs:** Tax strategy, entity structure recommendations, compliance calendar.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** MEDIUM — relevant once revenue is meaningful; not Phase 1.

### Investment Researcher
- **Source file:** `02-agents/library/agency-agents/finance/finance-investment-researcher.md`
- **Department:** Finance
- **Primary purpose:** Market research, due diligence, and asset valuation.
- **Expected inputs:** Investment target, research parameters, evaluation criteria.
- **Expected outputs:** Research report, risk assessment, valuation.
- **Likely tools required:** WebFetch, WebSearch, Read, Write
- **Relevance to AI Business Lab:** LOW — outside current scope.

---

## Product Department

### Trend Researcher
- **Source file:** `02-agents/library/agency-agents/product/product-trend-researcher.md`
- **Department:** Product / Strategy
- **Primary purpose:** Emerging trend identification, competitive analysis, and opportunity assessment.
- **Expected inputs:** Industry, focus area, competitive landscape.
- **Expected outputs:** Trend report, opportunity assessment, competitive map.
- **Likely tools required:** WebFetch, WebSearch, Read, Write, Edit
- **Relevance to AI Business Lab:** HIGH — market validation research before committing to Strategy A/B/C.
- **Overlap:** Partial overlap with `custom/business-research.md`. Trend Researcher is forward-looking; Business Research Agent is opportunity-scoring. Complementary.

### Product Manager
- **Source file:** `02-agents/library/agency-agents/product/product-manager.md`
- **Department:** Product
- **Primary purpose:** Full product lifecycle — discovery, roadmap, stakeholder alignment, go-to-market.
- **Expected inputs:** Product vision, user research, business goals, technical constraints.
- **Expected outputs:** Roadmap, PRD, go-to-market plan, outcome metrics.
- **Likely tools required:** WebFetch, WebSearch, Read, Write, Edit
- **Relevance to AI Business Lab:** HIGH — Tulboxx needs a product management layer as it adds features.

### Feedback Synthesizer
- **Source file:** `02-agents/library/agency-agents/product/product-feedback-synthesizer.md`
- **Department:** Product
- **Primary purpose:** Collect and synthesize user feedback into actionable product priorities.
- **Expected inputs:** Customer interviews, support tickets, survey responses, NPS data.
- **Expected outputs:** Prioritized insight report, feature request map, strategic recommendations.
- **Likely tools required:** WebFetch, WebSearch, Read, Write, Edit
- **Relevance to AI Business Lab:** HIGH — beta feedback from Tulboxx and Throttled Up clients needs synthesis.

### Sprint Prioritizer
- **Source file:** `02-agents/library/agency-agents/product/product-sprint-prioritizer.md`
- **Department:** Product
- **Primary purpose:** Agile sprint planning, feature prioritization, and resource allocation.
- **Expected inputs:** Feature backlog, team capacity, business priorities.
- **Expected outputs:** Sprint plan, prioritization rationale, velocity tracking.
- **Likely tools required:** Read, Write, Edit
- **Relevance to AI Business Lab:** MEDIUM — relevant for Tulboxx sprints; not Phase 1 priority.

### Behavioral Nudge Engine
- **Source file:** `02-agents/library/agency-agents/product/product-behavioral-nudge-engine.md`
- **Department:** Product
- **Primary purpose:** Adapts software interaction styles to maximize user motivation and success.
- **Expected inputs:** User behavior data, product goals, friction points.
- **Expected outputs:** Nudge strategy, interaction recommendations.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** LOW — premature for Phase 1.

---

## Engineering Department

### Multi-Agent Systems Architect
- **Source file:** `02-agents/library/agency-agents/engineering/engineering-multi-agent-systems-architect.md`
- **Department:** Engineering
- **Primary purpose:** Design, coordination, and governance of multi-agent AI pipelines.
- **Expected inputs:** Agent roster, task flows, failure scenarios, trust requirements.
- **Expected outputs:** Architecture diagram, coordination protocol, failure recovery plan.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** HIGH — directly applicable to building the AI-OS and agent orchestration.

### AI Engineer
- **Source file:** `02-agents/library/agency-agents/engineering/engineering-ai-engineer.md`
- **Department:** Engineering
- **Primary purpose:** ML model development, deployment, and AI-powered application integration.
- **Expected inputs:** AI use case, data requirements, integration targets.
- **Expected outputs:** AI feature design, integration plan, evaluation framework.
- **Likely tools required:** Bash, Read, Write, Edit
- **Relevance to AI Business Lab:** HIGH — building AI-powered delivery pipelines for Throttled Up and AI Business Lab.

### Prompt Engineer
- **Source file:** `02-agents/library/agency-agents/engineering/engineering-prompt-engineer.md`
- **Department:** Engineering
- **Primary purpose:** Crafting, testing, and optimizing prompts for production-grade AI behaviors.
- **Expected inputs:** AI task, failure cases, quality requirements.
- **Expected outputs:** Optimized prompt, test suite, evaluation framework.
- **Likely tools required:** Read, Write, Edit
- **Relevance to AI Business Lab:** HIGH — improving agent output quality is an ongoing task.

### Rapid Prototyper
- **Source file:** `02-agents/library/agency-agents/engineering/engineering-rapid-prototyper.md`
- **Department:** Engineering
- **Primary purpose:** Ultra-fast proof-of-concept development using efficient frameworks.
- **Expected inputs:** Feature concept, time budget, tech constraints.
- **Expected outputs:** Working prototype, implementation notes.
- **Likely tools required:** Bash, Read, Write, Edit
- **Relevance to AI Business Lab:** HIGH — Phase 1 validation requires fast prototypes to test offers.

### Backend Architect
- **Source file:** `02-agents/library/agency-agents/engineering/engineering-backend-architect.md`
- **Department:** Engineering
- **Primary purpose:** Scalable system design, database architecture, API development, and cloud infrastructure.
- **Expected inputs:** System requirements, scale targets, tech stack.
- **Expected outputs:** Architecture design, API specs, database schema.
- **Likely tools required:** Bash, Read, Write, Edit
- **Relevance to AI Business Lab:** HIGH — Throttled Up Platform and Tulboxx both need ongoing architecture support.

### Technical Writer
- **Source file:** `02-agents/library/agency-agents/engineering/engineering-technical-writer.md`
- **Department:** Engineering
- **Primary purpose:** Developer documentation, API references, README files, and tutorials.
- **Expected inputs:** Code, API specs, feature description.
- **Expected outputs:** Documentation, README, tutorial.
- **Likely tools required:** Read, Write, Edit
- **Relevance to AI Business Lab:** HIGH — agent definitions, playbooks, and internal docs all need quality documentation.

### Code Reviewer
- **Source file:** `02-agents/library/agency-agents/engineering/engineering-code-reviewer.md`
- **Department:** Engineering
- **Primary purpose:** Constructive code review focused on correctness, maintainability, security, and performance.
- **Expected inputs:** Code diff, PR description, code standards.
- **Expected outputs:** Code review comments, improvement recommendations.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** HIGH — Tulboxx and Throttled Up Platform need code quality oversight.

*(Additional engineering agents rated MEDIUM: Frontend Developer, Software Architect, Database Optimizer, DevOps Automator, Git Workflow Master, Minimal Change Engineer, Codebase Onboarding Engineer, Data Engineer, Email Intelligence Engineer, Payments & Billing Engineer, Identity & Access Engineer, Incident Response Commander, SRE, API Platform Engineer.)*

*(Engineering agents rated LOW: Embedded Firmware, WebAssembly, Network Engineer, Solidity/Blockchain, Section 508, USWDS, Drupal-specific, WordPress-specific, Feishu, WeChat Mini Program, Video Streaming, Desktop App, Mobile App, Mobile Release, i18n, OrgScript, FinOps, IT Service Manager, Filament Optimization, AI Data Remediation.)*

---

## Paid Media Department

### Paid Media Auditor
- **Source file:** `02-agents/library/agency-agents/paid-media/paid-media-auditor.md`
- **Department:** Marketing / Paid Media
- **Primary purpose:** Systematic evaluation of Google, Microsoft, and Meta ad accounts across 200+ checkpoints.
- **Expected inputs:** Ad account access or export, campaign history.
- **Expected outputs:** Audit report with prioritized recommendations.
- **Likely tools required:** WebFetch, WebSearch, Read, Write, Edit, Bash
- **Relevance to AI Business Lab:** HIGH — if running paid ads to acquire clients, auditing spend efficiency is critical.

### Paid Social Strategist
- **Source file:** `02-agents/library/agency-agents/paid-media/paid-media-paid-social-strategist.md`
- **Department:** Marketing / Paid Media
- **Primary purpose:** Cross-platform paid social advertising across Meta, LinkedIn, TikTok.
- **Expected inputs:** Campaign goal, budget, target audience, product/offer.
- **Expected outputs:** Campaign architecture, audience strategy, creative brief.
- **Likely tools required:** WebFetch, WebSearch, Read, Write, Edit, Bash
- **Relevance to AI Business Lab:** HIGH — Facebook/Instagram ads to contractors is likely the fastest paid channel.

### PPC Campaign Strategist
- **Source file:** `02-agents/library/agency-agents/paid-media/paid-media-ppc-strategist.md`
- **Department:** Marketing / Paid Media
- **Primary purpose:** Large-scale search, shopping, and Performance Max campaign architecture.
- **Expected inputs:** Campaign goals, budget, keywords, product/service.
- **Expected outputs:** Campaign structure, bid strategy, keyword plan.
- **Likely tools required:** WebFetch, WebSearch, Read, Write, Edit, Bash
- **Relevance to AI Business Lab:** MEDIUM — relevant if Google Ads is in scope for client acquisition.

### Ad Creative Strategist
- **Source file:** `02-agents/library/agency-agents/paid-media/paid-media-creative-strategist.md`
- **Department:** Marketing / Paid Media
- **Primary purpose:** Ad copywriting, RSA optimization, and creative testing frameworks.
- **Expected inputs:** Product/offer, target audience, platform, brand voice.
- **Expected outputs:** Ad copy variants, creative testing plan, asset recommendations.
- **Likely tools required:** WebFetch, WebSearch, Read, Write, Edit, Bash
- **Relevance to AI Business Lab:** MEDIUM — relevant when running paid ads; complements Paid Social Strategist.

### Search Query Analyst
- **Source file:** `02-agents/library/agency-agents/paid-media/paid-media-search-query-analyst.md`
- **Department:** Marketing / Paid Media
- **Primary purpose:** Search term analysis, negative keyword architecture, and query-to-intent mapping.
- **Expected inputs:** Search term report, campaign structure.
- **Expected outputs:** Negative keyword list, match type recommendations, query intent map.
- **Likely tools required:** WebFetch, WebSearch, Read, Write, Edit, Bash
- **Relevance to AI Business Lab:** MEDIUM — relevant for Google Ads optimization.

### Tracking & Measurement Specialist
- **Source file:** `02-agents/library/agency-agents/paid-media/paid-media-tracking-specialist.md`
- **Department:** Marketing / Paid Media
- **Primary purpose:** Conversion tracking architecture, tag management, and attribution modeling.
- **Expected inputs:** Business goals, tech stack, ad platforms.
- **Expected outputs:** Tracking implementation plan, GTM configuration, attribution model.
- **Likely tools required:** WebFetch, WebSearch, Read, Write, Edit, Bash
- **Relevance to AI Business Lab:** MEDIUM — important before scaling any paid acquisition.

### Programmatic & Display Buyer
- **Source file:** `02-agents/library/agency-agents/paid-media/paid-media-programmatic-buyer.md`
- **Department:** Marketing / Paid Media
- **Primary purpose:** Display advertising and programmatic media buying.
- **Expected inputs:** Campaign goal, budget, target audience, creative assets.
- **Expected outputs:** Media plan, targeting strategy, buying approach.
- **Likely tools required:** WebFetch, WebSearch, Read, Write, Edit, Bash
- **Relevance to AI Business Lab:** LOW — premature for Phase 1 budget level.

---

## Project Management Department

### Senior Project Manager
- **Source file:** `02-agents/library/agency-agents/project-management/project-manager-senior.md`
- **Department:** Operations
- **Primary purpose:** Converts specs to tasks, tracks scope, and remembers previous project context.
- **Expected inputs:** Project spec, timeline, team capacity.
- **Expected outputs:** Task list, schedule, scope boundary.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** HIGH — managing the Phase 1 to Phase 2 transition cleanly.

### Meeting Notes Specialist
- **Source file:** `02-agents/library/agency-agents/project-management/project-management-meeting-notes-specialist.md`
- **Department:** Operations
- **Primary purpose:** Extracts decisions, action items, and open questions from meeting transcripts.
- **Expected inputs:** Meeting transcript or rough notes.
- **Expected outputs:** Structured 4-section summary with decisions, actions, owners, and questions.
- **Likely tools required:** Read, Write, Edit
- **Relevance to AI Business Lab:** MEDIUM — useful for client calls and strategy sessions.

### Experiment Tracker
- **Source file:** `02-agents/library/agency-agents/project-management/project-management-experiment-tracker.md`
- **Department:** Operations
- **Primary purpose:** Manages A/B tests, feature experiments, and hypothesis validation.
- **Expected inputs:** Experiment hypothesis, success metrics, timeline.
- **Expected outputs:** Experiment log, results analysis, next action.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** MEDIUM — 7-day validation tests need systematic tracking.

### Project Shepherd
- **Source file:** `02-agents/library/agency-agents/project-management/project-management-project-shepherd.md`
- **Department:** Operations
- **Primary purpose:** Cross-functional project coordination, timeline management, and stakeholder alignment.
- **Expected inputs:** Project plan, stakeholder list, blockers.
- **Expected outputs:** Status update, risk log, stakeholder report.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** MEDIUM — relevant once there are multiple parallel builds.

*(Studio Operations and Studio Producer rated LOW — designed for creative production studios.)*

---

## Support Department

### Analytics Reporter
- **Source file:** `02-agents/library/agency-agents/support/support-analytics-reporter.md`
- **Department:** Support / Operations
- **Primary purpose:** Transforms raw data into dashboards, KPI tracking, and actionable business insights.
- **Expected inputs:** Raw data, KPI definitions, reporting period.
- **Expected outputs:** Dashboard design, KPI report, trend analysis.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** HIGH — MRR, churn, and conversion rate tracking from day one.

### Finance Tracker
- **Source file:** `02-agents/library/agency-agents/support/support-finance-tracker.md`
- **Department:** Finance / Support
- **Primary purpose:** Financial planning, budget management, and cash flow optimization.
- **Expected inputs:** Revenue, expenses, budget targets.
- **Expected outputs:** Financial summary, cash flow projection, budget variance.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** HIGH — tracking path to $5k and $10k MRR.

### Support Responder
- **Source file:** `02-agents/library/agency-agents/support/support-support-responder.md`
- **Department:** Support
- **Primary purpose:** Customer support, issue resolution, and experience optimization.
- **Expected inputs:** Customer message, product context.
- **Expected outputs:** Response, resolution action, escalation flag.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** MEDIUM — relevant once client volume requires systematic support.

### Legal Compliance Checker
- **Source file:** `02-agents/library/agency-agents/support/support-legal-compliance-checker.md`
- **Department:** Support / Legal
- **Primary purpose:** Ensures business operations comply with relevant laws and regulations.
- **Expected inputs:** Content or process description, jurisdiction.
- **Expected outputs:** Compliance assessment, flagged risks, remediation steps.
- **Likely tools required:** WebFetch, WebSearch, Read, Write
- **Relevance to AI Business Lab:** MEDIUM — useful when drafting client contracts.

### Infrastructure Maintainer
- **Source file:** `02-agents/library/agency-agents/support/support-infrastructure-maintainer.md`
- **Department:** Engineering
- **Primary purpose:** System reliability, performance optimization, and technical operations.
- **Expected inputs:** Infrastructure inventory, performance metrics, SLA targets.
- **Expected outputs:** Maintenance plan, performance report, optimization recommendations.
- **Likely tools required:** Bash, Read, Write
- **Relevance to AI Business Lab:** LOW — premature for Phase 1 scale.

---

## Testing Department

*(All testing agents are rated MEDIUM for Phase 1 — important for quality assurance of the delivery pipeline but not the first priority.)*

### Reality Checker
- **Source file:** `02-agents/library/agency-agents/testing/testing-reality-checker.md`
- **Department:** Testing
- **Primary purpose:** Evidence-based certification; defaults to "NEEDS WORK"; requires proof for production readiness.
- **Expected inputs:** Feature or product to evaluate.
- **Expected outputs:** Pass/fail verdict with specific evidence requirements.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** MEDIUM — useful before declaring any product "ready to sell."

### Tool Evaluator
- **Source file:** `02-agents/library/agency-agents/testing/testing-tool-evaluator.md`
- **Department:** Testing / Strategy
- **Primary purpose:** Evaluating and recommending tools, software, and platforms for business use.
- **Expected inputs:** Use case, evaluation criteria, shortlist of tools.
- **Expected outputs:** Evaluation scorecard, recommendation, implementation notes.
- **Likely tools required:** WebFetch, WebSearch, Read, Write
- **Relevance to AI Business Lab:** MEDIUM — useful when evaluating GHL vs. alternatives or AI tools.

### Workflow Optimizer
- **Source file:** `02-agents/library/agency-agents/testing/testing-workflow-optimizer.md`
- **Department:** Operations / Testing
- **Primary purpose:** Analyzes and optimizes business workflows for maximum efficiency.
- **Expected inputs:** Current workflow description, bottlenecks, goals.
- **Expected outputs:** Optimized workflow, automation opportunities, efficiency metrics.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** MEDIUM — useful for optimizing the AI content delivery pipeline.

*(Evidence Collector, Test Automation Engineer, API Tester, Performance Benchmarker, Test Results Analyzer, Accessibility Auditor rated LOW for Phase 1 — relevant for Tulboxx QA in later phases.)*

---

## Design Department

*(All design agents are rated LOW for Phase 1 except the four below.)*

### Brand Guardian
- **Source file:** `02-agents/library/agency-agents/design/design-brand-guardian.md`
- **Department:** Design / Marketing
- **Primary purpose:** Brand identity development, consistency maintenance, and strategic positioning.
- **Expected inputs:** Brand brief, existing assets, usage scenarios.
- **Expected outputs:** Brand guidelines, consistency audit, positioning recommendations.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** MEDIUM — relevant for OTW brand development.

### UX Researcher
- **Source file:** `02-agents/library/agency-agents/design/design-ux-researcher.md`
- **Department:** Design
- **Primary purpose:** User behavior analysis, usability testing, and data-driven design insights.
- **Expected inputs:** Product, user segments, research questions.
- **Expected outputs:** Research plan, usability findings, prioritized recommendations.
- **Likely tools required:** WebFetch, WebSearch, Read, Write
- **Relevance to AI Business Lab:** MEDIUM — relevant for improving Tulboxx contractor UX.

### Persona Walkthrough Specialist
- **Source file:** `02-agents/library/agency-agents/design/design-persona-walkthrough.md`
- **Department:** Design
- **Primary purpose:** Simulates cognitive walkthroughs from a persona's psychological perspective.
- **Expected inputs:** Web page or product, persona definition.
- **Expected outputs:** Emotional reaction map, CRO report, friction inventory.
- **Likely tools required:** WebFetch, Read, Write
- **Relevance to AI Business Lab:** MEDIUM — useful for optimizing the first landing page.

### UI Designer
- **Source file:** `02-agents/library/agency-agents/design/design-ui-designer.md`
- **Department:** Design
- **Primary purpose:** Visual design systems, component libraries, and interface creation.
- **Expected inputs:** Brand guidelines, functional requirements, component inventory.
- **Expected outputs:** Design specifications, component designs, style guide.
- **Likely tools required:** Read, Write
- **Relevance to AI Business Lab:** MEDIUM — relevant for Tulboxx UI improvements.

---

## Academic, Game Development, GIS, Healthcare, Security, Spatial Computing

These departments are rated LOW for AI Business Lab Phase 1. They are preserved in the library for future reference.

- **Academic** (6 agents): Anthropologist, Geographer, Historian, Narratologist, Psychologist, Statistician — useful for world-building research; not applicable to current business context.
- **Game Development** (19 agents): Not applicable.
- **GIS** (13 agents): Not applicable.
- **Healthcare** (3 agents): Not applicable.
- **Security** (10 agents): MEDIUM for Tulboxx — AppSec Engineer and Compliance Auditor become relevant when handling client data at scale.
- **Spatial Computing** (6 agents): Not applicable.

---

## Strategy Framework Documents (Not Agents)

These files contain playbooks, runbooks, and coordination templates rather than individual agent definitions. They have no frontmatter.

| File | Description |
|------|-------------|
| `strategy/nexus-strategy.md` | Master strategy coordination framework |
| `strategy/QUICKSTART.md` | Quick start guide for the agency-agents system |
| `strategy/EXECUTIVE-BRIEF.md` | Executive summary of the system |
| `strategy/coordination/agent-activation-prompts.md` | Standard prompts for activating agents |
| `strategy/coordination/handoff-templates.md` | Templates for agent-to-agent handoffs |
| `strategy/playbooks/phase-0-discovery.md` | Discovery phase playbook |
| `strategy/playbooks/phase-1-strategy.md` | Strategy phase playbook |
| `strategy/playbooks/phase-2-foundation.md` | Foundation phase playbook |
| `strategy/playbooks/phase-3-build.md` | Build phase playbook |
| `strategy/playbooks/phase-4-hardening.md` | Hardening phase playbook |
| `strategy/playbooks/phase-5-launch.md` | Launch phase playbook |
| `strategy/playbooks/phase-6-operate.md` | Operate phase playbook |
| `strategy/runbooks/scenario-enterprise-feature.md` | Enterprise feature runbook |
| `strategy/runbooks/scenario-incident-response.md` | Incident response runbook |
| `strategy/runbooks/scenario-marketing-campaign.md` | Marketing campaign runbook |
| `strategy/runbooks/scenario-startup-mvp.md` | Startup MVP runbook |

These documents are valuable references. The Chief of Staff should review `strategy/coordination/handoff-templates.md` and `strategy/coordination/agent-activation-prompts.md` when designing inter-agent workflows.

---

## Example Workflow Documents (Not Agents)

| File | Description |
|------|-------------|
| `examples/workflow-book-chapter.md` | Example of agents collaborating on a book chapter |
| `examples/workflow-landing-page.md` | Example of agents building a landing page |
| `examples/workflow-startup-mvp.md` | Example of agents launching an MVP |
| `examples/workflow-with-memory.md` | Example of agents using persistent memory |
| `examples/nexus-spatial-discovery.md` | Example of the Nexus coordination system |
