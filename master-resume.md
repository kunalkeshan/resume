# Master Resume

## Contact & Links

- **Name:** Kunal Keshan
- **Email:** kunalkeshan12@gmail.com
- **Phone:** +91 89398 81702
- **LinkedIn:** linkedin.com/in/kunalkeshan
- **GitHub:** github.com/kunalkeshan
- **Portfolio:** kunalkeshan.dev
- **Location:** Chennai, India

## Positioning Summary

Software engineer with a full-stack, infrastructure-leaning skill set: comfortable across React/Next.js frontends, Node.js/NestJS backends, CMS-driven content platforms, and GCP/AWS cloud infrastructure (IAM, CDNs, load balancers, Docker, CI/CD). Architected and built the NestJS backend for a live, production ride-hailing platform (Zion Taxi) end-to-end, including payments (Razorpay), RBAC/security, a fare-pricing engine, and a Jest-driven unit test suite (231 backend + 57 frontend spec files), alongside its React admin dashboard. Experience spans a fast-moving product/infra role at a multi-vertical startup, fintech contract work building AI-assisted tools, and a run of independent freelance builds across healthcare, e-commerce, hospitality, and personal branding. Comfortable owning a project end-to-end, from infra and backend to frontend and deployment, and equally comfortable going deep on one layer within a larger team. Open to full-stack, backend-leaning, or platform/infra-focused roles, at startups or larger organizations.

*[This is a keyword-rich reference summary for a master doc. Tailor sharply per role when generating a job-specific resume.]*

## Skills Bank

**Languages:** JavaScript (ES6+), TypeScript, Python, SQL, Bash/Shell, MATLAB, HTML5, CSS3

**Frontend/Mobile:** React.js, Next.js (App Router, SSG, ISR, on-demand revalidation), React Native, Expo, Module Federation (micro-frontend architecture), Tailwind CSS, shadcn/ui, Radix UI, Material UI, GSAP, Framer Motion / Motion, TanStack Query, Zustand, Redux, React Hook Form, Zod, Embla Carousel

**Backend:** Node.js, Express.js, NestJS, Python (FastAPI), Prisma ORM, Drizzle ORM, REST APIs, API architecture & design, Socket.io (realtime/WebSockets), FFMPEG (server-side video processing), ONNX Runtime (ML inference deployment)

**Testing:** Jest, ts-jest, Supertest, unit testing, test-driven development on service/business logic

**Payments & Security:** Razorpay (payment gateway integration), RBAC (role-based access control, permission grants, audit-actor coverage), WebAuthn, PII masking/data protection, CIDR-based access control

**CMS/Content:** Sanity, Payload CMS, Directus, Wix CMS API, Portable Text, React Email

**Cloud & Infrastructure:** Google Cloud Platform (IAM policies, load balancers, CDN, Compute Engine, Artifact Registry, Cloud Storage, secret management), AWS (S3, EC2, CloudFront), Cloudflare, Docker & Docker Compose (multi-stage builds, container networking, submodule-based builds), Nginx (reverse proxy, virtual hosts, TLS/ACME via Certbot), Vercel, Supabase, Grafana (agent-based monitoring)

**Auth & Security:** Auth0, Better Auth (multi-tenant RBAC via organization/admin plugins), Google Sign-In, Apple Sign-In, OAuth, Google reCAPTCHA v3

**AI/ML:** OpenAI API, IBM watsonx Orchestrate, LangChain, LangGraph (stateful agent orchestration), Retrieval-Augmented Generation (RAG) with pgvector (hybrid semantic + full-text retrieval), Langfuse (LLM observability/tracing, incl. self-hosted), adaptive filtering / signal processing (MATLAB), agentic assistant design

**Messaging/Integrations:** WhatsApp Cloud API (webhooks, interactive messages, Flow encryption), Telegram Bot API

**DevOps/Tooling:** Bash scripting & automation, GitHub Actions (CI/CD), Git submodules, build tagging & versioned deploys, Postman, Google Analytics (custom event tracking)

**Databases:** MongoDB, MySQL, PostgreSQL (via Prisma/Drizzle/Supabase), Redis

**Collaboration & Communication:** Cross-functional coordination (engineering and operations), developer mentorship, technical documentation (code-level, onboarding, business-facing), stakeholder communication, operations support

**Other:** Ngrok, web scraping, Nodemailer, i18n (next-intl), fuse.js (fuzzy string matching)

*[Bank is intentionally broad/redundant; mine for keyword overlap when tailoring, not meant to appear in full on any one resume.]*

## Experience

### StejasSYS
**Chennai, India (remote)**

Multi-vertical technology partner running product/infra work across hospitality, food & beverage, wellness, and ride-hailing clients, with operations in Atlanta, Ottawa, and Chennai. Kunal has held two sequential roles here (part-time to full-time conversion).

**Software Engineer (Full-time)** | Jan 2025 - Present
- Architected and built the NestJS backend for **Zion Taxi**, StejasSYS's in-house ride-hailing product, live in production with 300+ drivers, processing ~100 rides/month (outstation and one-way-drop trips). Owned module boundaries, the fare/pricing-strategy pattern, caching/coherency design, and the RBAC permission model end-to-end.
- Implemented the platform's transactional core: Razorpay payment gateway integration, commission/ledger settlement (GST-exclusive), and rider debt/balance resolution.
- Built a security-hardened access layer: RBAC with granular permission grants and audit-actor coverage, PII-masking interceptors, WebAuthn device-carry, and CIDR-based access restriction.
- Wrote and maintain the platform's unit test suite using Jest: 231 backend spec files (payments, RBAC/access control, fare pricing, PII masking, realtime WebSocket gateways) and 57 frontend test files on the companion React admin dashboard (permissions, fare display, booking/audit logic); ~3,700 individual test cases passing.
- Built the React 19/Next.js admin dashboard (`taxi-web-admin`) for internal ops: live trip tracking, fare/commission management, and driver/rider administration.
- Built the React Native/Expo driver and rider apps for Zion Taxi (the native client surface for the platform's 300+ drivers), including live GPS trip tracking and custom heading-calculation logic for smooth map navigation (device-heading smoothing for the driver app, route-direction-based fallback for the rider app), plus shared fare-breakdown logic reused across both apps.
- Built the conversation orchestration core, RAG-based knowledge retrieval system (pgvector), and admin API for **Innkraft's AI hotel sales agent**, a LangChain/LangGraph-powered WhatsApp/Telegram assistant handling guest conversations and booking flows for ~5 hotel clients (more onboarding). Built the Simplotel booking-provider integration (one of three live provider integrations) and a 60+ script regression-eval framework serving as the system's primary conversation-quality safety net.
- Own the company's cloud infrastructure end-to-end: GCP IAM policies, load balancers, CDNs, and secret management across the company's core product lines, including ride-hailing/taxi, hospitality (Innkraft, The Grand Regent), restaurant (Bytenosh, Culinex), and wellness/travel/Plugginn (an embeddable widget platform built on Module Federation for the embedding logic; handled deployment there and stayed closely involved in its architecture and planning).
- Built the 4-language (English, Tamil, Hindi, German) website for **The Grand Regent** hotel client using next-intl locale routing, migrating its CMS backend from Sanity to Payload as the platform evolved.
- Full-stack ownership of **Culinex**, an in-house restaurant operations platform (multi-outlet inventory, waste tracking, production-batch tracking, POS sales-data reconciliation) currently under active development, spanning frontend components, application routes, and the database schema.
- Designed and implemented the platform's RBAC foundation (Better Auth organization plugin with custom permission statements) for multi-tenant access control.
- Joined the platform's order-recommendation system (a cron-based restock-quantity model using consumption/waste/guest-count data) already in progress, and contributed to its planning and feature development going forward.
- Designed and documented an intelligent sales-data mapping system for reconciling CSV exports from external POS systems via fuzzy item matching, reusable across outlets and POS types.
- Led infrastructure and backend setup for multiple projects, including deploying and maintaining Directus CMS instances with build tagging, code freezing, and version control across environments.
- Migrated the shared reverse-proxy stack from a single monolithic Nginx config to a per-domain `conf.d/` structure (confirmed via `sys-proxy/nginx.conf.old`, 471 lines, vs. the current split config), improving maintainability across the company's multiple hosted domains.
- Built `update-service.sh`, a Bash automation that pulls a new versioned image tag from GCP Artifact Registry, updates the Docker Compose service definition, and restarts the affected containers, replacing a manual multi-step deploy with one command; used across the proxy repos (`sys-proxy`, `bytenosh-proxy`, etc.).
- Set up GitHub Actions CI/CD (confirmed live in `wellness-web` and `plugginn`) alongside Bash-based local dev/deploy tooling.
- Deployed and operate a computer-vision ML inference service (fingertip-video-based vitals estimation, built by a teammate) via containerized FastAPI, ONNX Runtime, GCS video storage, and an Nginx reverse-proxy layer.
- Authored technical documentation across three audiences: code-level references, developer onboarding guides, and business/feature-facing docs explaining shipped functionality in non-technical terms, reducing ambiguity for new engineers and non-technical stakeholders alike.
- Drafted a company-wide engineering standards handbook (Definition of Done, code review/testing/security practices, and role-based onboarding guides), scaffolded as a documentation site; a personal initiative, not yet formally adopted org-wide.
- Coordinated day-to-day with a ~3-5 person cross-functional engineering team and the on-site operations team running Zion Taxi's driver/rider operations, including ~2-3 months directly fielding operations support requests as the platform's engineer during the product's early rollout.
- Mentor new developers and drive continuous improvement in architecture, process, and team productivity while staying hands-on with engineering work.
- **Stack:** NestJS, Jest, Razorpay, RBAC/WebAuthn, Redis, Socket.io, Drizzle ORM, PostgreSQL, React 19, Next.js, GCP, Docker/Docker Compose, Nginx, Directus, GitHub Actions, Bash, LangChain, LangGraph, pgvector, WhatsApp Cloud API, Telegram Bot API, Langfuse, Better Auth, Prisma, fuse.js (fuzzy matching), React Native, Expo, react-native-maps, expo-location, Module Federation, FastAPI, ONNX Runtime

**Software Developer (Part-time)** | Jul 2024 - Dec 2024
- Built full-stack features using Next.js, TypeScript, Tailwind CSS, and Payload CMS, leading the transition from low-code tooling (Wix) to custom-built solutions.
- Implemented SSG with on-demand ISR and CMS webhook integrations for seamless content sync between Payload and the frontend.
- Diagnosed and fixed a major performance bottleneck: optimized image handling and disabled unnecessary prefetching, cutting page load time from **15s to 1-2s**.
- Reduced Docker image bloat via multi-stage builds, meaningfully improving build efficiency and deployment speed.
- Gained hands-on experience with GCP services (Compute Engine, Artifact Registry, Cloud Storage), Docker networking, and multi-environment pipelines with internal API routing for cost optimization.
- **Stack:** Next.js, TypeScript, Tailwind CSS, Payload CMS, Docker, GCP

### Flookup Capital Advisors (One21.ai)
**Contract Software Engineer** | Sep 2023 - Present
**Mumbai, India (remote)**

- Built and deployed custom websites and web apps for finance & tech clients, primarily Chartered Accountant-related services, under the One21.ai product umbrella.
- Led the transition from no-code platforms (e.g., Webflow ~$14/month) to custom Next.js deployments on Vercel, meaningfully cutting recurring hosting costs.
- Delivered dynamic CMS-driven solutions using Sanity, Payload, and Directus, letting non-technical client teams update content independently.
- Developed and scaled backend solutions on AWS, Supabase, and Vercel, including load balancers, S3 storage, and CloudFront CDN for optimized asset delivery.
- Implemented custom Google Analytics event tracking to capture business-specific user interactions and insights.
- Shipped multiple production solutions including:
  - **MCA Tech** ([mcatech.one21.ai](https://mcatech.one21.ai)): business intelligence platform with real-time financial data, risk assessments, and analytics across a database of 2.6M+ companies.
  - **CAGPT** ([cagpt.in](https://cagpt.in)): AI-powered platform delivering finance, taxation, compliance, and business-law guidance for accounting professionals.
  - **Snapshot** ([snapshot.one21.ai](https://snapshot.one21.ai)): business intelligence platform tracking funding trends and company data across 200+ companies.
  - **Merchant Banker** ([merchantbanker.in](https://merchantbanker.in))
  - **Flookup** ([flookup.com](https://flookup.com))
  - **Valuation Work** ([valuation.work](https://valuation.work))
  - **Captable**, **Due Diligence**, **Value Umbrella**, **GDS**, **Jobs**: additional One21.ai product suite tools
- **Stack:** Next.js, TypeScript, Sanity, Payload, Directus, AWS, Supabase, Vercel

### LingoScriptAI
**Product Development Engineer** | Jul 2023 - Mar 2024
**Chennai, India (remote)**

- Led development on a content-creation tool, working the full Agile cycle from research and development through deployment.
- Built the web application using TypeScript, Next.js, Tailwind CSS, Auth0, Node.js, and Express.js.
- Implemented FFMPEG for core functionality including server-side video rendering.
- Gained hands-on experience with AWS S3 and EC2, contributing to the tool's successful launch; collaborated closely with the team to resolve blockers quickly.
- No formal usage metrics captured for this role: primarily a fast-paced learning and shipping period.
- **Stack:** TypeScript, Next.js, Tailwind CSS, Auth0, Node.js, Express.js, FFMPEG, AWS

### Sundar Clinic
**Full-stack Developer** | Apr 2023 - Sep 2023
**Chennai, India**

- Built the clinic's responsive website from scratch, establishing its first proper online presence.
- Integrated Sanity CMS so clinic staff could update site content independently, without developer involvement.
- Introduced Tamil and Hindi localization (via next-intl) alongside the existing English site, extending reach to a wider local audience.
- Conducted performance optimization for faster page loads on sundarclinic.com.
- Contributed to a **~30% increase in clinic visits**, alongside a concurrent paid-ads push (the language localization work is believed to be a contributing factor, not the sole driver).
- **Stack:** Next.js, Sanity CMS, next-intl

### SRM University
**Project Assistant** | Nov 2022 - Mar 2023
**Chennai, India**

- Built a custom user interface (React, TypeScript, Axios) for a neural network model running on PYNQ Z-Series hardware, improving accessibility and interaction with the model.
- Collaborated with hardware engineers and medical professionals to integrate the UI successfully with the underlying hardware.
- Implemented secure Ngrok tunneling to reliably route traffic despite hardware limitations.
- **Stack:** React, TypeScript, Axios, Ngrok

### Blackwins Tech Solutions
**Frontend Developer (Intern)** | May 2022 - Jul 2022
**Chennai, India**

- Built user-facing interfaces for a SaaS product using React.js and Material UI, improving user engagement and satisfaction.
- Collaborated with designers and product managers to translate requirements into shipped features.
- Optimized performance to reduce server bandwidth usage during concurrent logins, improving load times and scalability.
- Conducted testing and debugging to resolve issues before release.
- No specific metric captured for this internship.
- **Stack:** React.js, Material UI

### Club & Community Leadership

*(Grouped separately from professional experience above: these were unpaid, community/student-org leadership roles run in parallel with coursework.)*

**IEEE SRMIST** | Oct 2021 - Sep 2023 *(2 years)*
- **Chairperson, Computer Society** (Feb 2023 - Sep 2023): Managed and mentored **50+ developers and AI/ML learners**; collaborated with industry experts to bring advanced AI/ML techniques into real-world projects; led several internal skill-building projects.
- **Technical Lead, Web and App Domain** (May 2022 - Feb 2023): Mentored **25+ developers**; led the technical side of **4+ events**, including building event websites and handling registrations.
- **Vice Lead, Web Domain** (Sep 2021 - Feb 2022): Led workshops on HTML, CSS, JS, Node.js, Express.js, Git/GitHub, and MySQL; mentored **10+ developers**; contributed to an internal club platform serving **200+ members**.
- **Web Developer** (Jan 2021 - Sep 2021, IEEE Webture track): Learned web development fundamentals; contributed to club projects; built a mini full-stack social media app (Node.js, Express.js, MySQL).

**Think-Digital, SRM** | Sep 2021 - Apr 2023 *(2 years 4 months)*
- **Team Head** (Oct 2022 - Apr 2023): Mentored and managed **40+ developers** on full-stack fundamentals and advanced concepts; ran weekly cross-team meetings with other domain leads; partnered with Think-Digital to bring in more internship opportunities for the team.
- **Web Domain Lead** (Feb 2022 - Oct 2022): Mentored **10 developers**; delivered **"Atom,"** an in-house project used by **200+ community members**; ran online workshops on frontend, backend, and Git/GitHub.
- **Vice Lead, Web Domain** (Sep 2021 - Feb 2022): a distinct, concurrent role from the same-titled IEEE SRMIST position above (confirmed the two ran in parallel on genuinely overlapping timelines, not a data error).

**SRMpedia**: **Web Developer**, Jan 2022 - Jul 2022
- Revived a broken mobile-app web scraper, restoring access to campus information for **3,000+ SRM students in KTR**.

**CodeChef SRM Student Chapter**: Web Developer, Dec 2021 - Jul 2022

## Projects/Freelance

*(Ordered newest to oldest by primary build/activity date. Kept to 1-2 tight bullets each: this section should scan as a compact list, not a second Experience section. Full detail for any entry can be pulled back out for tailoring if a JD calls for it.)*

### 9wealth: Personal Finance / Wealth Management App (unlaunched)
**Freelance, Full-stack (mobile, backend, and infra)** | Sep 2025 - Present

- Building (not yet launched) a personal finance app for tracking budget, investments, assets, and net worth, with an AI chat interface for spending/investment insights; built across React Native/Expo (mobile), NestJS/Prisma/Supabase (backend), and OpenAI API (AI trend-chat), with infrastructure owned end-to-end.
- **Stack:** React Native, Expo, NestJS, Prisma, Supabase, OpenAI API, TanStack Query

### Kumar Srivathsan: Portfolio Site
**Freelance, Full-stack** | Mar 2026

- Built a personal portfolio site for a maritime Navigation Officer, showcasing his career across container ships, Ro-Ro vessels, and international shipping routes. Live at [kumarsrivathsan.com](https://kumarsrivathsan.com).
- **Stack:** Next.js 16, TypeScript, Tailwind CSS, shadcn/ui, Vercel

### Community Knowledge Weaver: Agentic AI Assistant
**Hackathon project, IBM Dev Day "AI Demystified" Hackathon 2026** | Jan 2026

- Built an agentic AI assistant unifying scattered organizational knowledge (projects, tickets, policies, notes) into one chat interface on IBM watsonx Orchestrate, with a multi-agent orchestrator routing each question to the right specialist agent, able to both answer and take action (create tickets, add notes) via MCP tools.
- **Stack:** IBM watsonx Orchestrate, MCP (Model Context Protocol), TypeScript

### Keeping It Sou: Artist Website
**Freelance, Full-stack** | Jan 2026

- Built the official website for hip-hop artist Sou, showcasing releases, music, and upcoming drops, with Sanity CMS for content management. Live at [keepingitsou.com](https://keepingitsou.com).
- **Stack:** Next.js 16, TypeScript, Tailwind CSS, Sanity CMS, Vercel

### Dr. Nidhi: Portfolio Site
**Freelance, Full-stack** | Dec 2025

- Built a portfolio website for a doctor's practice, using GSAP and Framer Motion for polished page interactions.
- **Stack:** Next.js, TypeScript, Tailwind CSS, GSAP, Framer Motion

### Hzel Brown: Dessert Brand E-commerce (unlaunched)
**Side project, Full-stack** | Oct 2025 - Apr 2026

- Built (not yet launched) an e-commerce platform for an artisan dessert brand (handcrafted brownies, brookies, cupcakes, and cookies with delivery across Tamil Nadu), with full menu/cart/categorization, Sanity CMS webhook-driven revalidation, and React Email transactional templates.
- **Stack:** Next.js 16, React 19, TypeScript, Sanity CMS, Tailwind CSS, Radix UI, Zustand, React Email

### Jungli The Nomad: Wix CMS Video Carousel
**Freelance, Full-stack** | Jul 2024 - Dec 2025

- Built a custom, server-hydrated video testimonial carousel pulling content natively from **50+ videos** in the client's existing Wix CMS, embedded into their site via iframe, with lazy loading and infinite pagination for smooth playback across the carousel.
- **Stack:** Next.js 14, TanStack Query, Wix CMS/Data API, Embla Carousel

*(Additional smaller/older self-directed and academic projects, kept as a compact list per your steer, full detail available in each repo if needed for keyword mining:)*

- **Mind-Check** (2023-2026): Web app assessing emotional well-being via the Burns Depression Checklist.
- **Shiryoku** (2022-2025): Open-source curated resource list for upskilling across programming, design, and engineering.
- **Hardware Web UI** (2022-2024): Web-based GUI for interfacing with a breast cancer detection neural network.
- **Xilinx Homepage** (2023-2024): Site for SRMIST's Xilinx-funded Women in Technology (WIT) initiative.

## Education

**SRM Institute of Science and Technology**, Chennai, India
Bachelor of Technology (B.Tech), Electronics & Communication Engineering
Sep 2020 - May 2025 · CGPA: 8.65

**St. John's International Residential School**
Jul 2013 - Apr 2020

## Certifications & Courses

- **SQL for Data Science**, Coursera / UC Davis, Apr 2023
  Covers core SQL for data work: SELECT/filtering/sorting (WHERE, BETWEEN, IN, LIKE, ORDER BY, GROUP BY), subqueries, joins and unions, and data-manipulation functions for analysis (the foundational course in UC Davis's "Learn SQL Basics for Data Science" specialization).
- **Responsive Web Design**, freeCodeCamp, Aug 2021
  Project-based certification (15 practice projects + 5 certification projects, ~300 hours) covering semantic HTML, forms, accessibility, CSS Flexbox, and CSS Grid for fully responsive layouts.
- **M001: MongoDB Basics**, MongoDB University, Jan 2022
  6-chapter course covering MongoDB fundamentals vs. relational DBs, BSON/JSON, importing/exporting and querying data, document CRUD operations, indexing and the aggregation pipeline, and the Atlas/Compass tooling ecosystem.
- **Claude 101**, Anthropic Academy, Aug 2026 *(exact day pending)*
  Anthropic's foundational course on using Claude for everyday work tasks and understanding its core features and capabilities.
- **Claude Code 101**, Anthropic Academy, Aug 2026 *(exact day pending)*
  Anthropic's course on using Claude Code effectively within a daily development workflow.
- **Postman API Fundamentals Student Expert**, Postman, Dec 2022
- **Introduction to Systems Engineering**, Coursera, Nov 2022
- **Programming, Data Structures and Algorithms using Python**, NPTEL, Sep 2022 *(matches your GitHub repo `Programming-Data-Structures-and-Algorithms-using-Python-NPTEL-Course`)*
- **The Node.js Master Class**, Pirple, Jul 2022
- **Keeping Up With the JavaScripts: ES6**, Pirple, Jan 2022
- **Web Development**, Internshala, Oct 2021

## Awards/Recognition

### Publication
**"Leaky LMS Algorithm Based Low Complexity Adaptive Noise Cancellation"**
2025 International Conference on Recent Advances in Electrical, Electronics, Ubiquitous Communication, and Computational Intelligence (RAEEUCCI), Chennai, India, Apr 2025
DOI: [10.1109/RAEEUCCI63961.2025.11048209](https://doi.org/10.1109/RAEEUCCI63961.2025.11048209)
Authors: S. Maiti, D. Adusumalli, K. Keshan, S. Sharma, S. H. Pauline, S. Dhanalakshmi
Proposes a multistage Leaky LMS adaptive filtering approach for low-complexity noise cancellation in biomedical (PCG) and speech signals, applied to denoising speech recordings from Parkinson's-affected patients to improve diagnostic signal quality. Implemented in MATLAB (repo: `Leaky-LMS-Algorithm-Based-Low-Complexity-Adaptive-Noise-Cancellation`, built on earlier work in `PCG-Signal-Analysis-With-Adaptive-Filtering`, Aug 2024, confirmed as the precursor project).

### Other
*(Checked your LinkedIn export directly for Volunteering/Honors & Awards sections: it has neither; only Contact, Skills, Languages, Certifications, Publications, Summary, Experience, and Education. No award/recognition/volunteering content was found anywhere in the source material gathered. If there's something not on LinkedIn, let me know and I'll add it here.)*

## Extras

**Languages:** English (Full Professional), Tamil (Native/Bilingual), Hindi (Native/Bilingual), Japanese (Elementary)
