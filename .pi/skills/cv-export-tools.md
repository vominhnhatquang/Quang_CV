---
name: cv-export-tools
description: Choose rendering/export tools for CV Builder outputs
---

# CV Export Tools Skill

Use when adding PDF, DOCX, HTML, or Markdown export.

## Tooling options to evaluate

- HTML/CSS -> PDF via Playwright/headless Chromium: strong visual fidelity; used by modern resume builders such as Resume Matcher.
- Markdown -> PDF/DOCX via Pandoc: good for deterministic text-first pipelines and simple templates.
- DOCX templating: useful for recruiter-editable output, but requires careful style control.
- JSON Resume themes: useful inspiration for schema-driven theming and interchangeable layouts.

## Project defaults

- Start with text-first HTML/Markdown render payloads before PDF generation.
- Keep renderer input strictly typed and independent of LLM output.
- Provide an ATS-friendly single-column theme before decorative templates.
- Add snapshot/golden tests for rendered section order and key text.
