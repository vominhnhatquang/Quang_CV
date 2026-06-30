# Võ Minh Nhật Quang
**AI Engineer Intern Candidate | AI Systems & Full-stack ML Projects**
Ho Chi Minh City, Vietnam · +84 902 304 205 · vominhnhatquang@gmail.com · [GitHub](https://github.com/vominhnhatquang) · [Hugging Face](https://huggingface.co/Nhat-Quang)

## Summary
Second-year Artificial Intelligence student at FPT University, building practical AI systems across RAG, recommendation, model validation, data pipelines, and production-style web deployment. Strong learning mindset with hands-on Python/TypeScript projects, vector search, graph retrieval, QLoRA/LoRA adapters, and clear technical documentation.

## Education
- **FPT University HCMC** — Bachelor program in Artificial Intelligence (2024–2027)

## Skills
- **AI / ML:** RAG, hybrid search, Qdrant, BM25, model validation, regression, Qwen/Gemma LoRA, QLoRA, embeddings, retrieval evaluation
- **Backend / Data:** Python, FastAPI, Flask, Pydantic, PostgreSQL, Redis, Celery, Google Sheets API, data scraping, quality gates
- **Frontend / Deployment:** TypeScript, Next.js, React, Tailwind CSS, Vite, Docker Compose, Cloudflare Workers/OpenNext, GitHub Actions
- **Tools:** Git/GitHub, Hugging Face Hub, DVC, Makefile, Playwright, Vitest, ESLint, Photoshop, InDesign, Illustrator

## Selected Projects
### OutfitMatch — AI Fashion Stylist (2026)
*Private GitHub + public HF artifacts* · Python, Qdrant, graph retrieval, QLoRA, Qwen, fashion recommendation
- Built core data/knowledge-base path for a Vietnamese fashion recommendation system: catalog scraping, semantic item tagging, sparse item-compatibility graph, retrieval, quiz reranking, and size suggestions.
- Validated 5,618 catalog items and item-store links; latest audit reports 0 invalid rows and graph KB with 4,694 adult nodes and 316,559 canonical edges.
- Published Hugging Face artifacts for OutfitMatch LoRA adapters on Qwen/Gemma variants and a VN_Fashion_data dataset snapshot for reproducible project data.

### RAG Chatbot — Document Q&A (2026)
*Public* · FastAPI, Next.js, Qdrant, PostgreSQL, Redis, Docker, RAG · https://github.com/vominhnhatquang/MultiAgent_RAG
- Implemented a document Q&A system with PDF/DOCX/MD/TXT ingestion, Celery async processing, hybrid vector + BM25 retrieval, Reciprocal Rank Fusion, HyDE transform, strict guard threshold, and SSE streaming answers with citations.
- Designed a containerized 8-service architecture under a 10GB RAM budget, including FastAPI backend, Next.js frontend, Qdrant, PostgreSQL, Redis, Celery worker, and LLM routing.

### ORICAVI Coffee Website (2026)
*Private* · Next.js 15, React 19, TypeScript, Cloudflare, Playwright, Vitest
- Developed a static-first production website foundation with typed route/content boundaries, release-mode adapters, contact API seams, security/cache artifacts, and validation commands for lint, typecheck, tests, build, E2E smoke, and Lighthouse.
- Prepared Cloudflare Workers/OpenNext deployment flow with explicit preview/production build gates and secret-management boundaries.

### Gisdio CMS / Website Admin (2026)
*Private* · React, Vite, Node.js, Express, RBAC, CMS
- Built an admin dashboard for visual website content management, media/blog workflows, 3-role RBAC, live preview, and static HTML export.
- Structured frontend/backend modules with developer and user guides for maintainable handoff.

### Water Quality Prediction Web App (2026)
*Public* · Jupyter, scikit-learn, Flask, regression, GridSearchCV · https://github.com/vominhnhatquang/Predict-Jartest_N_SONG_KN-by-Antigravity
- Created an end-to-end ML pipeline for water-quality regression, comparing Linear/Ridge/Lasso/ElasticNet/Random Forest/Gradient Boosting models with reproducible 80/10/10 train-validation-test split.
- Exported trained model artifacts and exposed predictions through a Flask API with a responsive web interface.

### Hanet to Google Sheets Webhook (2025)
*Private* · Python, Flask, Google Sheets API, webhook, retry logic
- Implemented a webhook service that receives Hanet check-in/device/face/place events, validates hashes/IDs, de-duplicates events, retries Google Sheets writes, and logs operational details.

## Hugging Face Artifacts
- **VN_Fashion_data:** Dataset snapshot for OutfitMatch; 5,618 catalog items, Vietnamese fashion/e-commerce tags. (https://huggingface.co/datasets/Nhat-Quang/VN_Fashion_data)
- **OutfitMatch LoRA adapters:** Public PEFT/LoRA adapters for OutfitMatch stylist experiments on Qwen/Qwen-VL/Gemma variants. (https://huggingface.co/Nhat-Quang)