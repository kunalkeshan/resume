---
name: resume-tailor
description: Generate a tailored, job-specific resume from master-resume.md for a given job description. Use when Kunal pastes a job description and asks for a tailored/customized resume, or wants an existing tailored resume adjusted for a specific role.
---

# Resume Tailor

Generates a job-specific resume by selecting and reframing content from `master-resume.md` — never inventing it. This is Mode 2 from the project's `CLAUDE.md`; this skill formalizes that workflow.

## When to Use

- Kunal pastes a job description (JD) and asks for a tailored resume.
- He asks to adjust an existing application folder in `tailored/` for a slightly different angle on the same or a similar role.

## Core Principle: Highlight, Don't Fabricate

Tailoring means selecting and emphasizing the most relevant *true* content from `master-resume.md`, mirroring the JD's language where it's honestly accurate to what Kunal has done. It is never:
- Adding skills/tools he hasn't used
- Changing or inflating metrics
- Inventing experience, titles, or certifications
- Claiming a JD's exact keyword if the honest match is only adjacent

If `master-resume.md` doesn't support a claim the JD wants, leave it out — don't paper over the gap.

## Process

1. **Read `master-resume.md` fully.** This is the only source of factual content.
2. **Optionally check `references/`** if Kunal wants a specific style/structure mirrored — for formatting/phrasing inspiration only, never facts.
3. **Research the hiring company and, if applicable, the recruiter/staffing agency.** The JD sometimes comes via a third-party recruiter or staffing firm rather than the company itself (e.g. hiring "via" an agency) — identify both:
   - **The actual hiring company**: what it does/builds, industry, stage (startup/scale-up/enterprise), and anything relevant to positioning (e.g. fintech/regulated → emphasize security and compliance-adjacent work; product company → emphasize ownership and product thinking over pure contracting).
   - **The recruiter/staffing agency**, if the JD is routed through one rather than posted directly by the company: note it's a third-party channel, but tailor the resume content itself to the *end company*, not the agency, since the agency is just the intermediary.
   - If the JD gives little detail (common with agency-routed postings), do a quick web search on the company name/domain to fill gaps before tailoring. Use this research to sharpen the Positioning Summary and bullet selection, not to fabricate anything not in `master-resume.md`.
4. **Parse the JD** for: required/preferred skills, tools & technologies, seniority signals, core responsibilities, and the exact terminology used (e.g. "Kubernetes" vs "container orchestration").
5. **Select relevant content:**
   - Which Experience/Projects entries are most relevant, and in what order
   - Which bullets within each entry to lead with
   - Which Skills Bank items to surface (and phrase using the JD's terminology when accurate)
   - Which Certifications/Education items matter for this role
6. **Rewrite the Positioning Summary** specifically for this role — mirror the JD's language, lead with the most relevant strengths, and reflect the company research from step 3 (industry framing, product vs. agency-contract framing, etc.).
7. **Assemble the tailored resume** in ATS-safe format (see Format below).
8. **Length:** don't force a fixed page count — let content and seniority drive it. For senior/backend-heavy roles, default to 2 pages without asking. Ask Kunal only if the 1-page-vs-2-page call is genuinely ambiguous (e.g. an early-career JD).
9. **Save**, following the folder convention below.

## Format Requirements (ATS-Compatible)

- Single column, plain structure — applies to both `resume.md` and `resume.tex`
- Standard section headings: Summary, Experience, Skills, Education, Projects, Certifications
- No tables, text boxes, multi-column layouts, graphics, icons, or photos — in either output format
- Clean typography/spacing/emphasis is fine as long as it doesn't break ATS parsing on export
- **No em dashes ("—") anywhere** — headers, bullets, connecting clauses. They read as AI-generated. Use a period, comma, colon, or parentheses instead. A plain hyphen in a date range or compound adjective is fine.
- **One company, multiple roles → one header, nested role subheadings.** If a company has more than one sequential role in `master-resume.md` (promotion, title change, part-time-to-full-time conversion), render it as a single company heading with each role nested underneath as its own subheading + dates + bullets. Never split one company into two top-level Experience entries — it reads as two employers.
- **Projects section: 1-2 tight bullets per entry.** Keep it scannable, not a second Experience section. Core Experience entries can run fuller (2-4 bullets).

## Delivery: Folder Convention

Every tailored application is its own folder at `tailored/<company-slug>-<role-slug>-<date>/`:

- `<company-slug>` / `<role-slug>`: lowercase, spaces/punctuation → hyphens, parentheticals like "(Remote)" stripped. Ask Kunal for the company/role if either isn't obvious from the JD. If the JD is routed through a recruiter/staffing agency, slug the *end hiring company* (from step 3's research), not the agency name.
- `<date>`: `YYYY-MM-DD`, the folder's creation date — fixed at creation, not updated on later edits.
- Revisions to the same company + role + date: append `-rev2`, `-rev3`, ... rather than overwriting. A new date gets a fresh folder.
- Example: `tailored/stripe-staff-backend-engineer-2026-08-31/`

Each folder contains:

1. **`resume.md`** — the content source of truth for this application.
2. **`resume.tex`** — the same content in the default template, `templates/jakes-resume/` (Jake's Resume — verified ATS-safe: single column, no icons/graphics, includes `glyphtounicode` for clean text extraction). Use a different template from `templates/` only if Kunal asks for one by name.
   - **Self-contained templates** (`jakes-resume/`, `sb2nov-resume/` — a single `resume.tex`): copy that one file into the application folder as `resume.tex` and fill in its placeholders.
   - **Multi-file templates** (`russel-resume-ats-safe/` — `resume.tex` + `russell.cls` + `fonts/` + `cv/*.tex`, linked by relative paths): copy the *entire template folder's contents* into the application folder first (the `.cls`, `fonts/`, and `cv/` subfolder all need to sit next to `resume.tex`, not just the top-level file), then fill in `resume.tex` and each `cv/*.tex` placeholder. Copying only `resume.tex` produces a file that cannot compile.
   - Fill in the template's placeholders with content pulled straight from the already-assembled `resume.md` — don't re-derive content independently between the two formats, or they can drift.

No local PDF compilation — `.tex` source is the deliverable. Kunal compiles it himself (e.g. via Overleaf) when he wants a PDF.

## Keyword Integration Rules

**Do:**
- Use exact JD phrasing when it's truthfully accurate to his work
- Place important keywords in the Summary, Skills, and Experience bullets — not just one place
- Reorder Skills Bank entries so the most JD-relevant ones lead

**Don't:**
- Keyword-stuff (repeating the same term unnaturally)
- Force a keyword where it changes the meaning of what he actually did
- Sacrifice readability for density

## Output

After generating, briefly summarize for Kunal:
- The hiring company identified (and the recruiter/agency, if the JD was routed through one) and what the quick research turned up
- Which Experience/Projects entries were included and in what order
- What the rewritten Summary emphasizes
- Which keywords from the JD were incorporated (and honestly matched)
- Any JD requirements that `master-resume.md` doesn't support (so he knows the gap, rather than it being silently glossed over)
- The folder path, and which files were saved (`resume.md` and `resume.tex`)

Save the files — don't just print the resume in chat.
