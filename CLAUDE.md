# Resume Project

You are helping Kunal maintain a master resume and generate tailored, job-specific resumes from it. Everything lives locally as markdown in this directory:

- **`master-resume.md`** — the single source of truth. All content, facts, and history live here.
- **`references/`** — example/reference resumes (his own past resumes, or resumes he likes stylistically or structurally). Useful for formatting, structure, and phrasing inspiration when generating a tailored resume — but never a source of factual content. If it conflicts with `master-resume.md`, `master-resume.md` wins.
- **`tailored/`** — generated, job-specific resumes, one subfolder per application. Doesn't exist until the first one is created; created on demand (see Mode 2).
- **`templates/`** — reference LaTeX resume templates used to generate `resume.tex` in each tailored application folder. See Mode 2 for which is default.

## Two modes of work in this project

**1. Building/updating the master resume**

When Kunal describes new work, a project, a certification, a course, or an achievement:

- Read `master-resume.md` first so you don't duplicate or conflict with existing entries.
- Don't just log what he says verbatim. Ask follow-up questions until you have: what he did, the tools/tech/skills involved, and a quantified outcome or impact (a number, percentage, scale, or timeframe — whatever fits). If he can't quantify something precisely, ask for his best estimate rather than skipping it.
- Write the final entry as a blend: polished, action-verb-led, quantified resume language, while keeping it recognizably in his own voice rather than generic corporate-speak.
- For certifications/courses specifically, always capture: name, issuing body, date, key learnings/topics covered, and the specific skills/tools it involved — even though a final tailored resume will usually only show name + date. The extra detail exists so it can be mined for keyword overlap later.
- Update `master-resume.md` directly. Keep the doc organized under these sections, in this order:
  1. Contact & Links
  2. Positioning Summary
  3. Skills Bank
  4. Experience
  5. Projects/Freelance
  6. Education
  7. Certifications & Courses
  8. Awards/Recognition
  9. Extras (optional)
- **Experience** = formal jobs. **Projects/Freelance** = independent/freelance work (e.g. Sunder Clinic and similar self-directed work) — keep this in its own section, never mixed into Experience. Client/product work done as an employee (e.g. a StejasSYS client engagement) is Experience, never Projects, even if it resembles freelance work in shape.
- Every Experience/Projects entry should have: role/context, org, dates, a one-line scope, bullets in *what-you-did → tools touched → quantified outcome* form, and a short "stack used" tag line.
- **One company, multiple sequential roles:** if Kunal has held more than one role at the same company over time (a promotion, a part-time-to-full-time conversion, a title change), use a single company header (with location) and nest each role as its own subheading underneath, each with its own dates and bullets. Never give the same company two separate top-level entries — that reads as two different employers. This applies to any company, not just specific past examples.
- The Skills Bank should stay broad and redundant on purpose — include near-synonyms and tool variants, since it functions as a keyword bank for tailoring, not a polished final list.

## Style Guidelines (apply everywhere: master resume and tailored output)

- **No em dashes.** Em dashes ("—") read as AI-generated to reviewers. Rewrite sentences/clauses using periods, commas, colons, or parentheses instead. This applies to prose bullets, headers, and connecting clauses alike — don't reach for "—" as a default connector. A plain hyphen in a date range (e.g. "Jan 2025-Present") or a compound adjective is fine; it's the sentence-joining em dash that must go.
- **Projects/Freelance bullets: keep tight, 1-2 per entry.** This section should read as a scannable list, not a second Experience section. Core Experience entries can run fuller (2-4 bullets) since that's the primary substance of a resume, especially for senior roles.
- **Two pages is an accepted default for senior/backend-heavy roles.** For a senior-level JD or when Kunal's relevant experience is substantial, don't ask about page length before defaulting to 2 pages — go ahead and use it. Still ask if the role reads as junior/early-career, where 1 page may fit better.

**2. Generating a tailored resume for a specific job**

When Kunal gives you a job description (pasted in chat — it doesn't need to live in these instructions) and asks for a tailored resume:

- Read `master-resume.md`. Optionally check `references/` if Kunal wants a specific style/structure mirrored.
- Identify the role's key requirements, tools, and phrasing, and pull the most relevant Experience/Projects/Skills/Certifications entries — mirroring the JD's exact terminology where it's honestly true to what he's done (e.g. "Kubernetes," not "container orchestration," if the JD says Kubernetes and he's actually used it).
- Rewrite the positioning summary specifically for that role.
- **Length:** don't force a fixed page count. Default to whatever length the content and the role's seniority naturally support. For senior/backend-heavy roles, default to 2 pages without asking (see Style Guidelines above); ask Kunal only if the role or his experience level makes the call genuinely ambiguous (e.g. an early-career JD).
- **Format:** ATS-compatibility is the priority — single column, standard section headings (Experience, Skills, Education, etc.), no tables/text boxes/graphics/multi-column layouts. This applies equally to both output formats below — the LaTeX output must be just as ATS-safe as the markdown, never more decorative at the cost of parseability.
- **Delivery:** save every tailored application into its own folder at `tailored/<company-slug>-<role-slug>-<date>/`, containing:
  - `resume.md` — the markdown version (source of truth for content)
  - `resume.tex` — the same content rendered into the default LaTeX template (`templates/jakes-resume/`, unless Kunal asks for a different one from `templates/`)
  - No local PDF compilation — `.tex` source is the deliverable. Kunal compiles it himself (e.g. via Overleaf) when he wants a PDF.

  **Folder naming:**
  - `<company-slug>` and `<role-slug>`: lowercase, spaces and punctuation replaced with hyphens, parenthetical qualifiers like "(Remote)" stripped.
  - `<date>`: `YYYY-MM-DD`, the date the folder is first created — it does not change on later edits to the same application.
  - Example: a Staff Backend Engineer (Remote) application to Stripe on 2026-08-31 → `tailored/stripe-staff-backend-engineer-2026-08-31/`.
  - **Revisions:** if Kunal asks to redo/adjust an application for the same company + role on the same date, don't overwrite — append `-rev2`, `-rev3`, etc. to the folder name (e.g. `tailored/stripe-staff-backend-engineer-2026-08-31-rev2/`) so prior versions stay as history. A new date always gets a fresh, un-suffixed folder.
  - Ask Kunal for the company/role if either isn't obvious from the JD, so the slug is sensible.
- No need to keep a tracking log of past applications — Kunal manages that himself.

## Tone

Direct and practical. Ask clarifying/quantifying questions when adding master resume content — don't guess at metrics or skip the question because it feels like friction.
