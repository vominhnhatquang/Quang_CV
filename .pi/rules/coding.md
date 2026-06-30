# Coding Conventions — CV Builder

## Runtime

- Python >=3.13 as declared in `pyproject.toml`.
- Keep dependencies minimal until features require them.
- Prefer standard-library implementations for early schema validation, parsing, and CLI plumbing.

## Architecture

- Use a canonical structured resume representation inspired by JSON Resume: basics, work, education, skills, projects, certificates/awards, languages, interests.
- Keep job descriptions as separate structured inputs with title, company, raw text, extracted keywords, responsibilities, and requirements.
- Pipeline order: ingest -> validate -> analyze job -> tailor -> render -> review/export.
- Isolate any LLM provider behind an interface so local/offline logic remains testable.

## ATS and CV quality rules

- Default to one-column layouts and standard section headings.
- Avoid images, icons-only labels, tables-as-layout, and multi-column defaults for ATS-focused resumes.
- Preserve factual accuracy: never invent dates, employers, metrics, degrees, or certifications.
- Tailoring must reuse user-provided achievements and only rewrite for clarity, relevance, and measurable impact.

## Privacy

- Treat resumes, job descriptions, and contact info as sensitive personal data.
- Do not store secrets, API keys, uploaded resumes, or generated private resumes in `.pi/`.
- Prefer local files and explicit user opt-in for cloud LLM/API usage.

## Tests

- Add unit tests for schema validation, keyword extraction, scoring, and rendering payloads.
- Use deterministic fixtures; avoid live web/API calls in tests.
