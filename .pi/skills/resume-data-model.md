---
name: resume-data-model
description: Design and validate canonical resume/CV data before rendering or LLM tailoring
---

# Resume Data Model Skill

Use before implementing parsing, storage, tailoring, or export.

## Canonical sections

Model resumes using structured sections similar to JSON Resume:

- basics: name, label/headline, email, phone, url, location, profiles, summary
- work: company, position, location, start/end dates, summary, highlights
- education: institution, area, study type, dates, score, courses
- skills: name, level, keywords
- projects: name, description, highlights, keywords, url
- certificates/awards/publications/volunteer/languages/interests when needed

## Rules

- Validate required fields and date formats at ingest boundaries.
- Keep raw imported text separate from normalized structured data.
- Never let an LLM overwrite factual source data directly; require diff/suggestion review.
- Store tailored resumes as derived artifacts referencing the master profile and job description.

## Implementation preference

Start with Python dataclasses or Pydantic-style models only if dependency policy allows it. Keep JSON serialization stable for future themes/exporters.
