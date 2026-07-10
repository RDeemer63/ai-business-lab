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

### Claude-Powered GHL AI Layer (Webhook Architecture)
- Proposes: a lightweight webhook server that intercepts GHL inbound SMS, calls Claude API with contractor-specific context, and posts the AI reply back via GHL conversations API — replacing GHL's native Conversations AI with a Claude-powered equivalent
- Problem claimed: GHL's Conversations AI is UI-only (no API config), limiting our ability to set up and customize AI responses programmatically per contractor client
- Evidence needed: Gate 3 passes and at least one paying contractor client — at that point setup speed matters and the value of API-driven configuration is real
- Why it's better than GHL native: Claude outperforms GHL's LLM, prompts are fully customizable per client, the intelligence layer is owned by us not GHL, and new clients require only a new prompt not a new UI build
- Build estimate: ~100-line Node.js server, deploy free on Railway/Render, one GHL workflow built once in UI. Ryan has Vercel available.
- Parked: 2026-07-10

### Principle Registry (08-governance/PRINCIPLE_REGISTRY.md)
- Proposes: a registry where every operating principle records: principle text, status, origin experiment, origin decision, evidence link, supersedes, superseded by, last exercised date
- Problem claimed: principles lose their lineage as the organization grows; future agents cannot distinguish principles earned from evidence from principles adopted aspirationally
- Evidence needed: 10 or more principles in the operating system, with at least 2 documented instances where knowing a principle's origin would have changed a decision or prevented a mistake
- Parked: 2026-07-10

---

## Graduated Entries

_(none yet -- entries move here when they earn their way into the architecture)_
