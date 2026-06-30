---
name: ats-tailoring-review
description: Review and tailor resumes against job descriptions while preserving truthfulness and ATS readability
---

# ATS Tailoring Review Skill

Use when implementing or reviewing tailoring, scoring, or generated CV text.

## Tailoring loop

1. Extract job facts: title, company, must-have skills, nice-to-have skills, responsibilities, keywords, seniority, domain.
2. Map each job requirement to evidence in the master profile.
3. Rewrite only supported bullets; improve clarity, action verbs, and metric placement.
4. Flag gaps instead of inventing experience.
5. Score coverage with explainable matches/misses.

## ATS defaults

- Prefer one-column resume output.
- Use standard headings: Summary, Experience, Education, Skills, Projects, Certifications.
- Avoid graphics, photos, icon-only contact labels, text embedded in images, and layout tables.
- Keep bullets concise and accomplishment-oriented.

## Safety checks

- No fabricated employers, dates, degrees, certifications, tools, metrics, or responsibilities.
- Contact and personal data must not be sent to external APIs unless the user explicitly opts in.
- Keep a human-review step for any LLM-generated changes.
