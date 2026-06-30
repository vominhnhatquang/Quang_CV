---
name: cv-agent-research
description: Research-backed operating model for the CV Builder project agent
---

# CV Agent Research Baseline

Use this when designing features, data models, or prompts for CV/resume generation.

## Verified external references

- JSON Resume: open-source JSON-based resume standard for developers; useful as the canonical structured resume baseline. The archived `jsonresume/resume-schema` repo now points ongoing schema work to `jsonresume/jsonresume.org`, package `@jsonresume/schema` unchanged.
- Reactive Resume: free/open-source builder with instant PDF export, self-hosting via Docker, API access, multilingual support, templates, share links, and privacy-oriented positioning.
- OpenResume: free/open-source builder/parser, no sign-up, local browser storage, U.S. best-practice defaults, and ATS readability emphasis.
- Resume Matcher: open-source job-tailoring workflow: master resume + job description -> AI suggestions, scoring/keyword highlighting, cover letter generation, PDF export; supports local Ollama and cloud providers.

## Product direction for this repo

1. Store user career data once in a canonical structured profile.
2. Let job descriptions be first-class inputs, not prompt-only context.
3. Generate tailored resume variants from the master profile without mutating the master.
4. Provide review/scoring output that explains which job requirements are covered or missing.
5. Default to local/private behavior and make cloud model usage explicit.
