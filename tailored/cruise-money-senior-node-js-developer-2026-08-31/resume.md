# Kunal Keshan

kunalkeshan12@gmail.com · +91 89398 81702 · linkedin.com/in/kunalkeshan · github.com/kunalkeshan · kunalkeshan.dev · Chennai, Tamil Nadu, India

## Summary

Backend-leaning full-stack engineer specializing in Node.js and NestJS, with hands-on experience architecting and shipping a live, production financial-transaction system. Sole backend architect for a ride-hailing platform processing real payments via Razorpay, owning API architecture, a security-hardened RBAC/access-control layer, PII protection, and a thorough Jest-driven unit test suite across the backend and frontend. Comfortable across the full stack with React.js on the frontend, and experienced with AWS deployment (S3, EC2, CloudFront). Additional fintech exposure through contract work building AI-assisted tools for Chartered Accountant and financial-advisory clients. Product-first engineer who has owned systems end-to-end, from architecture and security design through backend, frontend, and deployment.

## Skills

**Languages:** JavaScript (ES6+), TypeScript, SQL, Python, Bash/Shell

**Backend:** Node.js, Express.js, NestJS, REST API design & architecture, Socket.io (realtime/WebSockets), Drizzle ORM, Prisma ORM

**Frontend:** React.js, React 19, Next.js, Tailwind CSS, TanStack Query, Zustand, Redux

**Testing:** Jest, ts-jest, Supertest, Unit Testing, test-driven development on service/business logic

**Payments & Security:** Razorpay (payment gateway integration), RBAC (role-based access control, permission grants, audit-actor coverage), Better Auth (multi-tenant RBAC), WebAuthn, PII masking/data protection, CIDR-based access control, Auth0, OAuth

**AI/LLM Systems:** LangChain, LangGraph (stateful agent orchestration), Retrieval-Augmented Generation (RAG) with pgvector, Langfuse (LLM observability/tracing), OpenAI API

**Cloud & Infrastructure:** AWS (S3, EC2, CloudFront), Google Cloud Platform (IAM, load balancers, CDN, Compute Engine), Docker & Docker Compose, Nginx, GitHub Actions (CI/CD), Redis

**Databases:** PostgreSQL (Drizzle/Prisma/Supabase), MongoDB, MySQL

**Collaboration & Communication:** Cross-functional coordination (engineering and operations), developer mentorship, technical documentation (code-level, onboarding, business-facing), stakeholder communication

## Experience

### StejasSYS
Chennai, Tamil Nadu, India

**Software Engineer (Full-time)** | Jan 2025 - Present
- Architected and built the NestJS backend for **Zion Taxi**, a live ride-hailing platform processing real payments (300+ active drivers, ~100 rides/month across outstation and one-way-drop trips), owning module boundaries, the fare/pricing-strategy pattern, caching/coherency design, and the RBAC permission model end-to-end.
- Implemented the platform's transactional core: Razorpay payment gateway integration, commission/ledger settlement (GST-exclusive), and rider debt/balance resolution, with correctness and auditability requirements for real-money flows.
- Built a security-hardened access layer: RBAC with granular permission grants and audit-actor coverage, PII-masking interceptors, WebAuthn device-carry, and CIDR-based access restriction.
- Wrote and maintain the platform's unit test suite using Jest: 231 backend spec files (payments, RBAC/access control, fare pricing, PII masking, realtime Socket.io gateways) and 57 frontend test files on the companion React admin dashboard (permissions, fare display, booking/audit logic); ~3,700 individual test cases.
- Built the conversation orchestration core, RAG-based knowledge retrieval system (pgvector), and admin API for **Innkraft's AI hotel sales agent**, a LangChain/LangGraph-powered WhatsApp/Telegram assistant handling guest conversations and booking flows for ~5 hotel clients; built one of three live booking-provider integrations and a 60+ script regression-eval framework serving as the system's primary conversation-quality safety net.
- Designed and implemented the RBAC foundation (Better Auth organization plugin with custom permission statements) for **Culinex**, an in-house restaurant operations platform, alongside full-stack ownership of its components, routes, and database schema.
- Own the company's cloud infrastructure: GCP IAM policies, load balancers, CDNs, Docker/Docker Compose deployments, and GitHub Actions CI/CD across the company's product lines.
- Authored technical documentation across code-level, developer onboarding, and business/feature-facing audiences, and coordinated day-to-day with a cross-functional engineering team (~3-5 people) and the on-site operations team running the platform's driver/rider operations.
- **Stack:** NestJS, TypeScript, Jest, Razorpay, RBAC/WebAuthn, Redis, Socket.io, Drizzle ORM, Prisma, PostgreSQL, LangChain, LangGraph, pgvector, Better Auth, React 19, Next.js, Docker, GCP, GitHub Actions

**Software Developer (Part-time)** | Jul 2024 - Dec 2024
- Built full-stack features using Next.js, TypeScript, Tailwind CSS, and Payload CMS, leading the transition from low-code tooling to custom-built solutions.
- Implemented SSG with on-demand ISR and CMS webhook integrations for seamless content sync.
- Diagnosed and fixed a major performance bottleneck: optimized image handling and disabled unnecessary prefetching, cutting page load time from 15s to 1-2s.
- Gained hands-on experience with GCP services (Compute Engine, Artifact Registry, Cloud Storage) and multi-environment deployment pipelines.
- **Stack:** Next.js, TypeScript, Tailwind CSS, Payload CMS, Docker, GCP

### Flookup Capital Advisors (One21.ai): Contract Software Engineer
Mumbai, Maharashtra, India (remote) · Sep 2023 - Present

- Built and deployed custom web applications for finance & tech clients, primarily Chartered Accountant-related fintech services, under the One21.ai product umbrella.
- Developed and scaled backend solutions on AWS and Supabase, including load balancers, S3 storage, and CloudFront CDN for optimized asset delivery.
- Delivered dynamic CMS-driven solutions letting non-technical client teams update content independently.
- Shipped production fintech-adjacent tools including **MCA Tech**, a business intelligence platform with real-time financial data and risk assessments across 2.6M+ companies, and **CAGPT**, an AI-powered platform delivering finance, taxation, and compliance guidance for accounting professionals.
- **Stack:** Next.js, TypeScript, AWS, Supabase, Vercel

### LingoScriptAI: Product Development Engineer
Chennai, Tamil Nadu, India · Jul 2023 - Mar 2024

- Built the web application backend using Node.js and Express.js, alongside a TypeScript/Next.js frontend and Auth0 authentication.
- Gained hands-on experience with AWS S3 and EC2, contributing to the tool's successful launch.
- **Stack:** TypeScript, Next.js, Node.js, Express.js, Auth0, AWS

## Projects

### 9wealth: Personal Finance / Wealth Management App (unlaunched)
Freelance, Full-stack (mobile, backend, and infra) · Sep 2025 - Present

- Building a personal finance app for tracking budget, investments, assets, and net worth, with an AI chat interface for spending/investment insights; backend built on NestJS, Prisma, and Supabase with OpenAI API integration, alongside a React Native/Expo mobile frontend.
- **Stack:** NestJS, Prisma, Supabase, OpenAI API, React Native, Expo

### Community Knowledge Weaver: Agentic AI Assistant
Hackathon project, IBM Dev Day "AI Demystified" Hackathon 2026 · Jan 2026

- Built an agentic AI assistant unifying scattered organizational knowledge into one chat interface on IBM watsonx Orchestrate, with a multi-agent orchestrator routing questions to specialist agents able to both answer and take action via MCP tools.
- **Stack:** IBM watsonx Orchestrate, MCP (Model Context Protocol), TypeScript

### Junglithenomad: Wix CMS Video Carousel
Freelance, Full-stack · Jul 2024 - Dec 2025

- Built a custom, server-hydrated video testimonial carousel pulling content natively from 2,500+ videos in the client's existing Wix CMS, with lazy loading and infinite pagination for performance across the large catalog.
- **Stack:** Next.js 14, TanStack Query, Wix CMS/Data API, Embla Carousel

## Education

**SRM Institute of Science and Technology**, Chennai, India
Bachelor of Technology (B.Tech), Electronics & Communication Engineering · Sep 2020 - May 2025 · CGPA: 8.65

## Certifications

- **Claude Code 101**, Anthropic Academy, Aug 2026
- **Claude 101**, Anthropic Academy, Aug 2026
- **The Node.js Master Class**, Pirple, Jul 2022
- **M001: MongoDB Basics**, MongoDB University, Jan 2022
- **SQL for Data Science**, Coursera / UC Davis, Apr 2023
