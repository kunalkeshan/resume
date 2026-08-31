# Resume

Kunal's master resume and a workflow for generating tailored, job-specific resumes from it, built to run with Claude Code.

Everything lives locally as markdown/LaTeX — no external resume builder, no tracking spreadsheet. One file holds the full career history; every application gets its own generated, ATS-safe resume pulled from that source.

## How it works

1. **`master-resume.md`** is the single source of truth — every job, project, skill, certification, and award Kunal has, written in full (unfiltered) detail.
2. When Kunal describes new work, Claude asks quantifying follow-up questions and adds a polished entry to the master resume.
3. When Kunal pastes a job description, Claude reads the master resume, pulls the most relevant entries, rewrites the positioning summary for that role, and generates a tailored resume — saved as both Markdown and ATS-safe LaTeX in its own folder under `tailored/`.

All the rules governing this (section order, quantification requirements, ATS formatting, folder naming, revision handling) are defined in [`CLAUDE.md`](CLAUDE.md).

## Project structure

```
master-resume.md   Single source of truth — all content and history
references/        Example resumes for style/structure inspiration (never factual content)
templates/          LaTeX resume templates used to render tailored resumes
tailored/           Generated, job-specific resumes — one folder per application
.claude/skills/     Claude Code skills that drive the workflow
```

### `master-resume.md`

Organized into a fixed section order: Contact & Links, Positioning Summary, Skills Bank, Experience, Projects/Freelance, Education, Certifications & Courses, Awards/Recognition, Extras. Experience (formal jobs) and Projects/Freelance (independent/freelance work) are kept strictly separate. The Skills Bank is intentionally broad and redundant — it's a keyword bank for tailoring, not a polished list.

### `references/`

Kunal's own past resumes or resumes he likes stylistically. Used for formatting/structure/phrasing inspiration only — `master-resume.md` always wins on factual content.

### `templates/`

Vetted, single-column, ATS-safe LaTeX templates used to render each tailored resume:

| Template | Default? | Notes |
|---|---|---|
| `jakes-resume/` | **Yes** | The de facto standard for US tech ATS resumes. |
| `russel-resume-ats-safe/` | No | Multi-file template (`russell.cls`, `fonts/`, `cv/*.tex`) with a modified icon-free, plain-hyperlink header. |
| `sb2nov-resume/` | No | Jake's Resume's direct ancestor; similar structure, different spacing/typography. |

See [`templates/README.md`](templates/README.md) for compiling details.

### `tailored/`

One subfolder per application, named `tailored/<company-slug>-<role-slug>-<date>/`, each containing:
- `resume.md` — markdown source of truth for that application's content
- `resume.tex` — the same content rendered into the default (or requested) LaTeX template

No PDFs are compiled locally — `resume.tex` is the deliverable; compile it yourself (e.g. via [Overleaf](https://www.overleaf.com/)) when you want a PDF.

## Usage

This project is designed to be driven conversationally through Claude Code, using the skills in [`.claude/skills/`](.claude/skills/):

- **Add to the master resume** — describe a new job, project, certification, or achievement in chat. Claude will ask for the tools/tech involved and a quantified outcome, then write the entry into `master-resume.md`.
  - `resume-bullet-writer` — turn a rough description of work into a single polished, quantified bullet.
- **Generate a tailored resume** — paste a job description and ask for a tailored resume. Claude pulls the relevant Experience/Projects/Skills, rewrites the summary, and saves `resume.md` + `resume.tex` under `tailored/`.
  - `resume-tailor` — drives the full tailoring workflow end to end.
  - `resume-ats-optimizer` — check an existing tailored resume's ATS compatibility and keyword match against a JD.
- **Redo an application** — ask to adjust an existing tailored resume for the same company/role/date; Claude appends `-rev2`, `-rev3`, etc. rather than overwriting.

All formatting stays ATS-compatible: single column, standard section headings, no tables/text boxes/graphics/multi-column layouts — in both the Markdown and LaTeX outputs.

## Getting started

```bash
git clone <this-repo>
cd resume
claude
```

Then just talk to Claude — describe your work to build up `master-resume.md`, or paste a job description to generate a tailored resume.
