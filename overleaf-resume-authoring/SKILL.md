---
name: overleaf-resume-authoring
description: Create, edit, or troubleshoot a LaTeX resume maintained in Overleaf. Use for project structure, source edits, compilation choices, links, and layout; not for inventing resume content.
metadata:
  short-description: Maintain an Overleaf LaTeX resume
---

# Overleaf resume authoring

Maintain an Overleaf resume as a small, stable LaTeX project whose content is easy to tailor and whose PDF is easy to scan.

## Inspect before changing

Read the existing main source, class/style files, compiler setting if known, and project file layout. Preserve the established template and dependencies unless the request calls for a redesign. Keep the main `.tex` file in the project root and make it the Overleaf Main document; this avoids compilation-path and auxiliary-file problems. Read [the project reference](references/overleaf-projects.md) for compiler, links, and debugging details.

## Authoring decisions

- Keep content and presentation separated when that makes repeated tailoring safer: reusable commands or a class/style file may hold stable presentation; source data or sections may hold role-specific content. Do not refactor a working one-file resume merely for abstraction.
- Default to the project compiler. For a new conventional Latin-script resume, pdfLaTeX is a sound default. Switch to XeLaTeX or LuaLaTeX only when the project needs OpenType/TrueType fonts, robust Unicode, or non-Latin scripts; update incompatible font/encoding packages at the same time.
- Preserve real text as selectable text. Do not use graphics, tables, columns, icons, colour, or spacing tricks in ways that hide essential information or make the document fragile.
- Use `hyperref` deliberately for contact and portfolio links. Prefer readable label text, `\href{...}{...}` or `\url{...}`, and unobtrusive link colours; check every final link in the PDF. Load `hyperref` late unless a documented package exception applies.
- Escape LaTeX-special characters in supplied content and use semantic section titles. Avoid manual line breaks and negative spacing as the first response to overflow.

## Verify

Compile after substantive source changes. Resolve errors and warnings that affect output, then inspect the rendered PDF at normal viewing size for one-page/target-length fit, clipping, awkward line breaks, consistent alignment, link behavior, and actual text selection. If local TeX is unavailable, give exact Overleaf steps and do not claim compilation succeeded.

Do not modify claims without candidate-provided evidence. Use `$resume-content-strategy` or `$resume-job-tailoring` for content decisions.
