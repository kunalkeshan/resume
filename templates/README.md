# Resume LaTeX Templates

Reference templates used by `resume-tailor` to generate `resume.tex` for each tailored application. All three are vetted single-column, ATS-safe (no images, icons rendered only as plain hyperlinked text where applicable, no page-level multi-column layouts).

| Template | Default? | Source | Notes |
|---|---|---|---|
| [`jakes-resume/`](jakes-resume/) | **Yes** | [github.com/jakegut/resume](https://github.com/jakegut/resume) (MIT) | The de facto standard for US tech ATS resumes. Includes `\input{glyphtounicode}`, which keeps ligatures extractable as clean text by ATS parsers. |
| [`russel-resume-ats-safe/`](russel-resume-ats-safe/) | No | Modified from [github.com/themagicalmammal/Resume](https://github.com/themagicalmammal/Resume) | Upstream uses a `\photo{}`-driven header and FontAwesome icons for social links. This variant never calls `\photo{}` (the class collapses that region to 0-width, so the header renders as a single column) and replaces icon-based contact links with plain hyperlinked text (bare URL as display text, e.g. `linkedin.com/in/...`) via `\extrainfo{}`, matching Kunal's own resume convention. See the header comment in `resume.tex` for the exact diff from upstream. **Multi-file template** — `russell.cls`, `fonts/`, and `cv/*.tex` must all be copied alongside `resume.tex` (see `resume-tailor/SKILL.md`). The `cv/*.tex` section files ship as `<placeholder>` stubs, not the upstream author's original resume content — fill them in per application. |
| [`sb2nov-resume/`](sb2nov-resume/) | No | [github.com/sb2nov/resume](https://github.com/sb2nov/resume) (MIT) | Jake's Resume's direct ancestor — very similar single-column structure, slightly different spacing/typography. Useful as a minor style variant. |

## Usage

`resume-tailor` fills in a template's placeholders with content from the already-generated `resume.md` for that application and saves `resume.tex` as source — no local PDF compilation is part of the workflow. See [`CLAUDE.md`](../CLAUDE.md) and [`.claude/skills/resume-tailor/SKILL.md`](../.claude/skills/resume-tailor/SKILL.md) for the full workflow.

## Compiling to PDF (optional, on your own)

If you want a PDF from a given `resume.tex`, the simplest route is pasting it into [Overleaf](https://www.overleaf.com/) (upload the whole template folder for `russel-resume-ats-safe/`, since it needs `russell.cls`, `fonts/`, and `cv/*.tex` alongside it — see that template's row above).

To compile locally instead, BasicTeX needs these packages beyond its default install:

```bash
sudo tlmgr install fullpage titlesec marvosym enumitem fontawesome5 roboto sourcesanspro tcolorbox xifthen biblatex biber
```

`fullpage`, `titlesec`, `marvosym`, `enumitem` are needed by `jakes-resume/` and `sb2nov-resume/`. `fontawesome5`, `roboto`, `sourcesanspro`, `tcolorbox`, `xifthen`, `biblatex`, `biber` are additionally needed by `russel-resume-ats-safe/` (`biblatex`/`biber` are pulled in unconditionally by `russell.cls` even though this variant cites nothing).
