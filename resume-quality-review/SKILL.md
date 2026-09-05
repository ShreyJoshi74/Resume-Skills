---
name: resume-quality-review
description: Audit a resume or compiled resume PDF for factual integrity, role relevance, ATS-readable structure, and visual defects. Use for review and prioritized fixes; do not silently rewrite claims.
metadata:
  short-description: Audit content, ATS, and PDF quality
---

# Resume quality review

Audit the final resume as a recruiter, an applicant-tracking parser, and a human PDF reader. Keep review separate from authorship so issues remain visible.

## Review order

1. **Truth and privacy:** Flag unsupported claims, ambiguous ownership, misleading titles or dates, inconsistent metrics, sensitive information, and links that need confirmation. Do not assume a claim is true because it sounds plausible.
2. **Target fit:** Compare the resume with the stated role or job description. Identify the strongest evidence, missing must-haves, irrelevant space, and terminology that can be used truthfully.
3. **Readable structure:** Check that contact details, headings, roles, employers, dates, education, skills, and project evidence are ordinary selectable text in a logical order. Flag excessive columns, icons in place of labels, text boxes, images of text, invisible keywords, or unexplained acronyms when they obstruct parsing or human scanning. Standard headings, standard fonts, and a conventional work-history structure are the least risky format when an application must be parsed by an ATS.
4. **Rendered PDF:** Inspect page count, whitespace balance, font size, line wraps, clipping, alignment, punctuation, dates, Unicode glyphs, URLs, and clickable links. Review at normal screen size and, if feasible, a print preview.

## Report

Give findings in priority order: blocking, high impact, polish. Each finding must state the location, why it matters, and the smallest safe remedy. Preserve candidate voice and facts. If changes are requested, route writing to `$resume-content-strategy` or `$resume-job-tailoring`, and LaTeX changes to `$overleaf-resume-authoring`.
