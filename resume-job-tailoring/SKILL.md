---
name: resume-job-tailoring
description: Tailor an existing resume for a specific role using a job description and verified candidate evidence. Use for relevance and keyword decisions, not to fabricate qualifications or change LaTeX styling.
metadata:
  short-description: Tailor a resume honestly to a role
---

# Resume job tailoring

Produce a role-specific resume variant that improves relevance without overstating the candidate.

## Inputs and comparison

Use the job description, the current/master resume, and any candidate clarifications. Extract the role's outcomes, required and preferred capabilities, domain language, seniority signals, location or authorization requirements, and application constraints.

Map each important requirement to one of: direct evidence, adjacent/transferable evidence, no evidence, or unclear. Do not turn an adjacent match into a direct claim. Ask targeted questions only for high-value unclear requirements.

## Tailor responsibly

- Reorder and condense existing evidence before adding new prose.
- Mirror job terminology only where it accurately describes the candidate's work. Preserve the candidate's actual job titles and credentials.
- Make the summary optional: include it only when it clarifies the fit more effectively than the first experience entry.
- Surface the strongest matching achievements early, while retaining enough non-targeted context for the resume to make sense.
- Keep standard sections and readable headings; keyword coverage must not become a keyword list or hidden text.
- Follow the employer's stated format, length, and location instructions when provided.

## Output

Provide (1) the requirement-to-evidence mapping, (2) the revised text or a precise change set, and (3) any unresolved gaps. Route source changes to `$overleaf-resume-authoring` when the resume is maintained in Overleaf.
