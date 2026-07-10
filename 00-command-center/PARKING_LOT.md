# Parking Lot

Ideas that have not earned their way into the architecture. A parked idea is not rejected. It is waiting for evidence.

To graduate from the parking lot: name the experiment that demonstrated the need. Then open an ADR.

---

## Format

Each entry follows this structure:

**[Short title]**
- Proposes: what structural change this would make
- Problem claimed: what problem this is supposed to solve
- Evidence needed: what experiment would validate the need
- Parked: date

---

## Current Entries

### Studio Health Dashboard
- Proposes: a dashboard showing business validation velocity, experiment completion rate, agent utilization, and kill rate
- Problem claimed: Ryan cannot quickly assess studio performance without reading multiple files
- Evidence needed: two operating months of data showing that the current file-based approach creates decision delays or missed signals
- Parked: 2026-07-09

### Orchestration Layer
- Proposes: an automated system that routes tasks between agents based on workflow type without Ryan manually initiating each agent session
- Problem claimed: Ryan has to manually trigger agent sessions, creating a bottleneck
- Evidence needed: G1 and G2 gates cleared (core agent quality validated) + documented evidence from Experiment Zero that manual routing is slowing launch velocity
- Parked: 2026-07-09

### Intelligence Department Formal Structure
- Proposes: a named Intelligence Department with its own README, role definitions, and formal reporting structure
- Problem claimed: intelligence functions (research, analysis, pattern recognition) are scattered across agents with no unified home
- Evidence needed: three or more workflows that would demonstrably benefit from coordinated intelligence functions in a shared department context
- Parked: 2026-07-09

### Weekly Rhythm Cadence
- Proposes: a formalized weekly cadence (Monday architecture review, Wednesday business pipeline, Friday lessons review) with automated prompts
- Problem claimed: without a rhythm, work happens reactively rather than systematically
- Evidence needed: four operating weeks showing that the absence of a cadence caused missed decisions or stale state
- Parked: 2026-07-09

### Maturity Level Tracking
- Proposes: a formal maturity level system (L1-L4) tracking the studio's progression from human-led to AI-led across research, validation, and launch functions
- Problem claimed: progress is invisible without a formal framework to measure it
- Evidence needed: six operating months of data to understand what milestones are actually meaningful vs. theoretical
- Parked: 2026-07-09

---

### Two-Speed Studio (Research Track / Build Track)
- Proposes: formally separating experiments into a fast Research Track (many ideas, rapid validation) and a slow Build Track (few ideas, high quality execution)
- Problem claimed: without separation, the studio risks spreading resources across too many simultaneous builds
- Evidence needed: two or more simultaneous active ventures where resource conflict is documented — or four completed experiments showing a natural split between ideas that validated quickly and ideas that required sustained build effort
- Parked: 2026-07-10

### AI Conversation Engine (Capability)
- Proposes: a reusable capability that generates context-aware, business-rule-driven conversations across any communication channel — designed to be portable across GHL, Tulboxx, future CRMs, email, web chat, voice, and messaging platforms
- Problem claimed: no programmable AI conversation layer exists in the current stack; GHL's native Conversations AI is UI-only and not configurable via API
- Use cases this capability powers: lead follow-up, estimate follow-up, review requests, invoice reminders, maintenance reminders, appointment confirmations, customer reactivation — lead follow-up (Experiment 001) is the first use case, not the definition of the capability
- Portability note: first implementation routes SMS through GHL; the capability is not defined by this implementation and should survive any change in CRM, AI model, or channel — including future portability into Tulboxx
- Evidence needed: Gate 3 passes and at least one paying contractor client — setup speed and programmability become real constraints at that point
- First implementation estimate: ~100-line webhook server, one GHL UI workflow built once, deploy free on Railway/Render or Ryan's Vercel
- Parked: 2026-07-10

### Capability Decision Matrix (Four-Question Buy/Build Framework)
- Proposes: a formal decision matrix applied to every capability discussion — four questions: Can we buy 80% today? Does it differentiate the studio? Does it improve every future experiment? Does it become organizational knowledge?
- Problem claimed: buy-vs-build decisions are currently made by feel; the matrix makes them consistent and traceable
- Evidence needed: at least 3 capability decisions where the matrix would have changed or validated the outcome — only then does a formal document earn its place over the heuristic already in CAPABILITY_LAYER_HEURISTIC.md
- Parked: 2026-07-10

### Four Compounding Assets Framework (Principles / Workflows / Capabilities / Recipes)
- Proposes: formally recognizing four classes of organizational asset that compound across experiments — Principles (how we decide), Workflows (how work moves), Capabilities (what we can do), Recipes (how to repeat success)
- Problem claimed: the studio accumulates assets without a shared vocabulary for what kind of asset each thing is — this creates confusion when deciding what to preserve vs. what to discard
- Evidence needed: at least one Recipe in the wild (a validated, reusable playbook extracted from a completed experiment) — until then the abstraction is theoretical
- Parked: 2026-07-10

### Feature Library (Observed / Correlated / Predictive Buying Signals)
- Proposes: a library where every experiment contributes structured features that predict buying behavior — starting as "observed," graduating to "correlated" when patterns emerge across experiments, and "predictive" when they reliably forecast conversion
- Problem claimed: interview data is currently captured as prose and lost after each experiment; structured features would make it queryable and compound across experiments
- Evidence needed: at least 40 structured interviews across 3+ experiments — only then does the pattern analysis become meaningful
- Note: the Gate 2 interview guide now captures structured features (Feature Capture table) — this is the seed, not the library
- Parked: 2026-07-10

### Signal-Based Prospect Discovery (Behavioral Signals Over Industry Classification)
- Proposes: identifying prospects based on observable behavioral signals — hiring office staff, launching Google Ads, adding locations, review velocity increase, website redesign, adding trucks, posting jobs — rather than industry + company size alone
- Problem claimed: industry classification finds the right category of buyer; behavioral signals find buyers at the right moment — the combination dramatically improves conversion rates
- Evidence needed: Year 2 capability. First need the Prospect Recipe Library from 5+ completed experiments, then map which signals correlated with conversion. Some free signals (GBP posts, review velocity, Facebook ad activity) can be tested earlier via Clay enrichment.
- Parked: 2026-07-10

### Calibration Metric (Studio-Level Confidence Accuracy)
- Proposes: tracking whether the studio's confidence scores are calibrated — when the studio says 80% confident, how often is it actually right? Produces a calibration curve comparing predicted confidence to actual outcomes.
- Problem claimed: confidence scores per experiment are useful for learning, but without calibration tracking, there is no way to know whether the studio is systematically overconfident, underconfident, or well-calibrated
- Evidence needed: at least 5 completed experiments with recorded confidence scores and actual outcomes — only then can a calibration curve be meaningful
- Note: per-experiment confidence tracking is the right behavior now; studio-level calibration is the next-order metric that makes confidence meaningful at scale
- Parked: 2026-07-10

### Principle Registry (08-governance/PRINCIPLE_REGISTRY.md)
- Proposes: a registry where every operating principle records: principle text, status, origin experiment, origin decision, evidence link, supersedes, superseded by, last exercised date
- Problem claimed: principles lose their lineage as the organization grows; future agents cannot distinguish principles earned from evidence from principles adopted aspirationally
- Evidence needed: 10 or more principles in the operating system, with at least 2 documented instances where knowing a principle's origin would have changed a decision or prevented a mistake
- Parked: 2026-07-10

---

## Graduated Entries

_(none yet -- entries move here when they earn their way into the architecture)_
