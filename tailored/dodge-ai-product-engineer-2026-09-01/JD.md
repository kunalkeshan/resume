# Product Engineer

**Company:** Dodge AI (apply via https://binary.so/5mCoci4)
**Hiring via:** Direct (Dodge AI posting)
**Compensation:** ₹25-50L CTC (in-hand + ESOPs), Full-Time
**Experience:** 1-4 YoE
**Location:** On-site, HSR Layout, Bengaluru, India. Six-day work week (Sundays off).

## Requirements

- Product judgement: asks why before how, has made real build decisions (not just execution), scopes honestly, has strong interface/UX taste.
- Interface engineering: ships screens end-to-end without a designer, has built streaming/real-time interfaces (SSE, WebSockets, partial output, interruption, reconnection), manages complex client/server state and optimistic updates, treats performance as a habit.
- Systems and data: can design an API from a feature description, knows REST vs. webhooks vs. streaming vs. queue vs. cache, uses standard patterns (pagination, rate limiting, retries/backoff, idempotency, connection pooling), designs schemas that hold up at scale, gets auth/tenant isolation right.
- Shipping and operating: has run live services with real customers (releases, rollouts, rollbacks), writes tests that are actually relied on, can fix CI, instruments what they build, can debug under time pressure in unfamiliar code.
- AI/agent work: benchmarking harnesses, context engineering (what goes in the context window and in what order, in-context learning, compaction/memory across long runs, tool design, just-in-time retrieval), building evaluation infrastructure that turns "I think this got better" into evidence.
- Default working environment is Claude Code, Codex, or Cursor (not a novelty) with real opinions on where each falls short.
- Good to have: LLM features shipped to real users (streaming/structured output/agentic flows), eval infrastructure for AI systems, a design system/component library adopted by other teams, durable workflow systems (Temporal/Celery) in production, integrations with awkward auth or hostile rate limits, any exposure to SAP or another ERP.
- Ideal profile: went deep on something hard and ended up in the top 1% at it (e.g. founder/founding engineer at an early-stage startup with real users/revenue, standout open-source contributions).

**Stack (one TypeScript monorepo):** Web: Next.js, React, Tailwind, shadcn, TanStack Query. API/Workers: Hono, tRPC, Node, Postgres with Drizzle. Agents: custom-built harnesses, sandboxing, MCP, skills, persisted state in Postgres. Around it: Docker, Better Auth, OpenTelemetry.

## Company Notes (research)

Dodge AI is building an AI platform for enterprise systems: agents that investigate, plan, and carry out changes across the standard enterprise software stack (SAP, Salesforce, Dynamics 365, Kinaxis, Ariba, Coupa, and the surrounding integrations), the work currently done by armies of systems-integrator consultants ($100B+/year industry). The hard problem they're solving is capturing the undocumented, company-specific logic layered on top of standard ERP/enterprise software.

Backed by Accel and Google's AI Futures Fund as part of the Atoms AI Cohort 2026 (Accel Atoms + Google AI Futures Fund India program, kicked off at Google Ananta, Bengaluru, March 2026). Publicly described focus: autonomous AI agents for ERP maintenance and modernization, aimed at spotting/resolving SAP AMS tickets and enhancements before they escalate, effectively substituting for traditional ERP-consultant spend. Cohort startups receive co-investment (~$2M split between Accel and Google AI Futures Fund) plus Google Cloud/Gemini/DeepMind compute credits. Small, founder-heavy team; live with Fortune 500 customers; offices in Bengaluru (HSR Layout) and San Francisco.

Sources: [Meet The 5 Startups In Google's AI Futures Fund & Accel's Atoms AI Cohort 2026](https://inc42.com/buzz/meet-the-5-startups-in-googles-ai-futures-fund-accels-atoms-ai-cohort-2026/), [Accel Atoms and Google's AI Futures Fund Announce AI Cohort 2026](https://atoms.accel.com/news/meet-the-startups-in-ai-cohort-2026)
