# Joaquin Peñafiel

**Backend & Applied AI | Python • FastAPI • JavaScript/Node.js • SQL • APIs • Observability • Docker • CI** 

I build backend services, API integrations, automation and applied AI systems with a focus on reliability, traceability and evidence-based engineering decisions.

My background combines software development with data/process transformation in operational environments.

## Featured project

### AI API Observability

Production-deployed FastAPI service for external API and AI-provider integration, with explicit reliability, observability and failure-handling controls.

**Links**

- [Live Dashboard](https://ai-api-observability-production.up.railway.app/dashboard)
- [Repository](https://github.com/joaquinpenafiel/ai-api-observability)
- [Architecture & Engineering Decisions](https://github.com/joaquinpenafiel/ai-api-observability/blob/main/docs/ARCHITECTURE.md)
- [API Documentation](https://ai-api-observability-production.up.railway.app/docs)

The project includes direct Gemini and Anthropic HTTP integrations, retries/backoff, request tracing, HMAC-SHA256 webhooks, SQL-backed telemetry, token/cost tracking, Docker, CI and 38 automated tests.

A dedicated load probe separated HTTP-layer degradation from SQLite write contention. Follow-up controlled experiments showed that WAL mode combined with persistent worker-local connections moved the measured persistence boundary substantially, delivering approximately 3.7x–4.4x more successful-write throughput across the tested concurrency range while reducing lock errors and latency. The optimization improved the boundary but did not eliminate contention at higher concurrency.

## Core technologies

**Backend:** Python, FastAPI, JavaScript/Node.js, REST APIs, httpx, Webhooks

**Data:** SQL, MySQL, SQLite, data migration, validation and normalization

**Reliability & Delivery:** pytest, structured logging, request tracing, Docker, GitHub Actions, Railway

**Applied AI:** AI-provider integrations, token/cost telemetry, provider normalization and failure handling

## Professional focus

Backend Engineering • Applied AI • API & Systems Integration • Automation • Data-intensive Systems • Reliability & Observability

I value explicit engineering trade-offs, reproducible experiments and systems whose behavior can be inspected and tested.

[LinkedIn](https://www.linkedin.com/in/joaquin-penafiel/)
