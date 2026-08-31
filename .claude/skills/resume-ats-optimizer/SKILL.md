---
name: resume-ats-optimizer
description: Check a tailored resume for ATS (Applicant Tracking System) compatibility and keyword match against a job description. Use when Kunal asks to check/optimize a resume for ATS, wants a match score against a JD, or asks why applications aren't getting responses.
---

# Resume ATS Optimizer

Audits a resume (typically `resume.md` or `resume.tex` inside an application folder under `tailored/`, or a draft in chat) for ATS-parsing safety and keyword match against a job description.

## When to Use

- Kunal asks to check ATS-compatibility of a resume
- He wants a keyword match score against a specific JD
- He's asking why a resume isn't getting responses

## What Breaks ATS Parsing

- Tables, multi-column layouts, text boxes, headers/footers holding contact info
- Non-standard section headers (anything other than recognizable names like "Experience," "Skills," "Education," "Summary")
- Images/graphics/charts, or text embedded in images
- Inconsistent date formats
- Non-standard fonts/special characters (only relevant if exporting beyond markdown)

Since this project keeps tailored resumes single-column and plain-structure (both `resume.md` and `resume.tex`) per `CLAUDE.md`, most structural ATS risk is avoided by default — check for regressions if a file has drifted from that (e.g. a markdown table added for skills, a LaTeX template swapped in that uses multi-column/icon/photo elements, etc).

## Keyword Match Process

1. **Read the JD** (paste provided in chat) and extract three keyword types:
   - **Hard skills**: languages, tools, platforms, certifications, methodologies
   - **Soft skills**: leadership, communication, stakeholder management, etc.
   - **Industry terms**: domain-specific vocabulary (e.g. SaaS, B2B, specific compliance terms)
2. **Read the resume file** and check each JD keyword for:
   - Exact phrase match
   - Synonym/variant match (flag these — may want the exact JD term instead, if honest)
   - Frequency and location (Summary / Skills / Experience)
3. **Calculate match score**: `(keywords matched / total JD keywords) × 100`. Target 80%+ for a strong match, but never suggest adding a keyword that isn't truthfully supported by `master-resume.md` — that's `resume-tailor`'s job to resolve honestly, not this skill's job to paper over.

## Output Format

```markdown
# ATS COMPATIBILITY REPORT — <file>

## Formatting Check
✅/❌ Single column, no tables/graphics
✅/❌ Standard section headers
✅/❌ Consistent date formatting
✅/❌ Contact info in body, not header/footer

## Keyword Match: X%

**Matched:**
- keyword — found Nx (location)

**Missing (present in JD, absent in resume):**
- keyword — appears Nx in JD

**Near-matches (consider aligning wording if honestly accurate):**
- resume says "X" / JD says "Y"

## Recommendations
- [specific, actionable — e.g. "add 'stakeholder management' to the Sunder Clinic bullet about X, if accurate"]
```

## Important Boundary

This skill **diagnoses**, it doesn't fabricate. If a missing keyword isn't truthfully supported by `master-resume.md`, say so explicitly rather than suggesting the resume claim it. Flag it as a genuine gap — Kunal may want to build that skill/experience, not fake it.
