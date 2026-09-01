# Kunal Keshan

kunalkeshan12@gmail.com · +91 89398 81702 · linkedin.com/in/kunalkeshan · github.com/kunalkeshan · kunalkeshan.dev

## Summary

Full-stack TypeScript engineer who has shipped a production LLM agent end to end: conversation orchestration, RAG retrieval, and the evaluation harness that keeps it honest. Architected and owns the NestJS backend for a live ride-hailing platform (300+ drivers, real payments) alongside its React admin dashboard, backed by a ~3,700-test Jest suite. Comfortable moving across the whole stack, from Postgres schema to React UI to Docker/GCP infra, and treats Claude Code as a daily tool rather than a novelty. Looking for a product-engineering role where judgment on what to build carries as much weight as how it gets built.

## Skills

**Languages:** TypeScript, JavaScript (ES6+), Python, SQL, Bash/Shell

**Frontend:** React.js, Next.js (App Router, SSG, ISR, on-demand revalidation), Tailwind CSS, TanStack Query, Zustand, Redux, React Hook Form, Zod

**Backend:** Node.js, Express.js, NestJS, REST API design & architecture, Socket.io (realtime/WebSockets), Drizzle ORM, Prisma ORM

**AI/Agent Systems:** LangChain, LangGraph (stateful agent orchestration), Retrieval-Augmented Generation (RAG) with pgvector (hybrid semantic + full-text retrieval), Langfuse (LLM observability/tracing), MCP (Model Context Protocol), OpenAI API, agentic assistant design

**Auth & Security:** Better Auth (multi-tenant RBAC via organization/admin plugins), RBAC (permission grants, audit-actor coverage), WebAuthn, OAuth, Auth0, PII masking/data protection

**Testing:** Jest, ts-jest, Supertest, unit testing, test-driven development on service/business logic

**Cloud & Infrastructure:** Google Cloud Platform (IAM, load balancers, CDN, Compute Engine, secret management), Docker & Docker Compose, Nginx, AWS (S3, EC2, CloudFront), GitHub Actions (CI/CD), Redis

**Databases:** PostgreSQL (Drizzle/Prisma/Supabase), MongoDB, MySQL

**Collaboration & Communication:** Cross-functional coordination (engineering and operations), developer mentorship, technical documentation (code-level, onboarding, business-facing), stakeholder communication

## Experience

### StejasSYS
Chennai, India (remote)

**Software Engineer (Full-time)** | Jan 2025 - Present.
- Built the conversation orchestration core, RAG-based knowledge retrieval (LangChain/LangGraph with pgvector hybrid search), and admin API for **Innkraft's AI hotel sales agent**, a WhatsApp/Telegram booking assistant serving ~5 hotel clients; built a 60+ script regression-eval framework as the system's primary conversation-quality safety net, with Langfuse instrumentation across the pipeline.
- Architected and built the **NestJS** backend for **Zion Taxi**, a live production ride-hailing platform (300+ drivers, ~100 rides/month), owning module boundaries, the fare-pricing engine, RBAC, and Razorpay payment integration end-to-end, plus its React 19 admin dashboard.
- Designed the platform's multi-tenant RBAC foundation using Better Auth's organization plugin with custom permission statements, layering in WebAuthn device-carry and PII-masking interceptors for a security-hardened access layer.
- Wrote and maintain a **~3,700-test** Jest suite (231 backend + 57 frontend spec files) covering payments, RBAC, fare pricing, and realtime Socket.io gateways.
- Own the company's cloud infrastructure end-to-end: GCP IAM policies, load balancers, CDNs, Docker/Docker Compose, Nginx, and GitHub Actions CI/CD across the company's product lines.
- **Stack:** NestJS, TypeScript, LangChain, LangGraph, pgvector, Langfuse, Better Auth, Drizzle ORM, PostgreSQL, Jest, Razorpay, RBAC/WebAuthn, Socket.io, React 19, Next.js, Docker, GCP, GitHub Actions.

**Software Developer (Part-time)** | Jul 2024 - Dec 2024.
- Built full-stack features using Next.js, TypeScript, Tailwind CSS, and Payload CMS, leading the transition from low-code tooling to custom-built solutions.
- Implemented SSG with on-demand ISR and CMS webhook integrations for seamless content sync between Payload and the frontend.
- **Stack:** Next.js, TypeScript, Tailwind CSS, Payload CMS, Docker, GCP.

### Flookup Capital Advisors (One21.ai)
Mumbai, India (remote)

**Contract Software Engineer** | Sep 2023 - Present.
- Delivered custom production web apps for finance & tech clients under the One21.ai product umbrella, including [CAGPT](https://cagpt.in), an AI-powered platform delivering finance, taxation, and compliance guidance for accounting professionals.
- Led the transition from no-code tooling to custom Next.js deployments on Vercel, meaningfully cutting recurring hosting costs, and developed backend solutions on AWS and Supabase (load balancers, S3, CloudFront CDN).
- **Stack:** Next.js, TypeScript, Sanity, AWS, Supabase, Vercel.

### LingoScriptAI
Chennai, India (remote)

**Product Development Engineer** | Jul 2023 - Mar 2024.
- Led development on a content-creation tool through the full Agile cycle, from research and development through deployment, using TypeScript, Next.js, Node.js, and Express.js.
- Implemented FFMPEG for core product functionality, including server-side video rendering, and shipped on AWS S3/EC2.
- **Stack:** TypeScript, Next.js, Node.js, Express.js, FFMPEG, Auth0, AWS.

## Projects

### Community Knowledge Weaver: Agentic AI Assistant
Hackathon project, IBM Dev Day "AI Demystified" Hackathon 2026 · Jan 2026.

- Built an agentic AI assistant unifying scattered organizational knowledge into one chat interface on IBM watsonx Orchestrate, with a multi-agent orchestrator routing questions to specialist agents that can both answer and take action via MCP tools.
- **Stack:** IBM watsonx Orchestrate, MCP (Model Context Protocol), TypeScript.

### 9wealth: Personal Finance / Wealth Management App (unlaunched)
Freelance, Full-stack (mobile, backend, and infra) · Sep 2025 - Present.

- Building a personal finance app with an AI chat interface for spending/investment insights (OpenAI API), across a React Native/Expo frontend and a NestJS/Prisma/Supabase backend, with infrastructure owned end-to-end.
- **Stack:** React Native, Expo, NestJS, Prisma, Supabase, OpenAI API, TanStack Query.

### Kumar Srivathsan: Portfolio Site
Freelance, Full-stack · Mar 2026.

- Built and shipped a personal portfolio site end-to-end using Next.js 16 and shadcn/ui components, live at [kumarsrivathsan.com](https://kumarsrivathsan.com).
- **Stack:** Next.js 16, TypeScript, Tailwind CSS, shadcn/ui, Vercel.

## Education

**B.Tech, Electronics & Communication Engineering** | Sep 2020 - May 2025.
SRM Institute of Science and Technology · CGPA: 8.65.

## Certifications

- **Claude Code 101**, Anthropic Academy, Aug 2026.
- **Claude 101**, Anthropic Academy, Aug 2026.
- **Postman API Fundamentals Student Expert**, Postman, Dec 2022.
