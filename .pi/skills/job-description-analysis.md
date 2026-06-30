---
name: job-description-analysis
description: Parse and score job descriptions for resume tailoring
---

# Job Description Analysis Skill

Use when building features that ingest job posts or compare resumes to jobs.

## Extract

- Role title, company, location/remote hints.
- Required skills and qualifications.
- Preferred/nice-to-have skills.
- Responsibilities and domain keywords.
- Seniority signals and years-of-experience expectations.

## Score

- Separate hard requirements from soft/preferred terms.
- Use explainable keyword and semantic matches.
- Penalize unsupported claims rather than rewarding hallucinated matches.
- Return missing evidence prompts: what the user should add if true.

## Output shape

Return structured JSON-like data with `requirements`, `keywords`, `matched_evidence`, `gaps`, and `suggested_resume_focus`.
