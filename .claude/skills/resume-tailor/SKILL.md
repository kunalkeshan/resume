---
name: resume-tailor
description: Generate a tailored, job-specific resume from master-resume.md for a given job description. Use when Kunal pastes a job description and asks for a tailored/customized resume, or wants an existing tailored resume adjusted for a specific role.
---

# Resume Tailor

Generates a job-specific resume by selecting and reframing content from `master-resume.md` — never inventing it. This is Mode 2 from the project's `CLAUDE.md`; this skill formalizes that workflow.

## When to Use

- Kunal pastes a job description (JD) and asks for a tailored resume.
- He asks to adjust an existing file in `tailored/` for a slightly different angle on the same or a similar role.

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
3. **Parse the JD** for: required/preferred skills, tools & technologies, seniority signals, core responsibilities, and the exact terminology used (e.g. "Kubernetes" vs "container orchestration").
4. **Select relevant content:**
   - Which Experience/Projects entries are most relevant, and in what order
   - Which bullets within each entry to lead with
   - Which Skills Bank items to surface (and phrase using the JD's terminology when accurate)
   - Which Certifications/Education items matter for this role
5. **Rewrite the Positioning Summary** specifically for this role — mirror the JD's language, lead with the most relevant strengths.
6. **Assemble the tailored resume** in ATS-safe format (see Format below).
7. **Length:** don't force a fixed page count — let content and seniority drive it. If the 1-page-vs-2-page call is ambiguous for this role/his experience level, ask.
8. **Save** to `tailored/<company-or-application-name>.md`. Ask for the company/application name if it isn't obvious from the JD.

## Format Requirements (ATS-Compatible)

- Single column, plain markdown structure
- Standard section headings: Summary, Experience, Skills, Education, Projects, Certifications
- No tables, text boxes, multi-column layouts, or graphics
- Clean typography/spacing/emphasis is fine as long as it doesn't break ATS parsing on export

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
- Which Experience/Projects entries were included and in what order
- What the rewritten Summary emphasizes
- Which keywords from the JD were incorporated (and honestly matched)
- Any JD requirements that `master-resume.md` doesn't support (so he knows the gap, rather than it being silently glossed over)

Save the file — don't just print the resume in chat.
