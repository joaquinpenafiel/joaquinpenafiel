# Joaquin Peñafiel

**Backend & Applied AI | Python • FastAPI • JavaScript/Node.js • SQL • APIs • Observability • Docker • CI**

I build backend services, API integrations, automation and applied AI systems
with a focus on reliability, traceability and evidence-based engineering
decisions.

My background combines software development with data/process transformation in
operational environments.

---

## Featured projects

Two projects of different kinds. One is a deployed service measured under load;
the other is a closed experimental program whose audit chain can be verified in
ten seconds. Both are built on the same habit: measure, isolate, and claim only
what the measurement supports.

---

### AI API Observability

Production-deployed FastAPI service for external API and AI-provider
integration, with explicit reliability, observability and failure-handling
controls.

**Links**

- [Live Dashboard](https://ai-api-observability-production.up.railway.app/dashboard)
- [Repository](https://github.com/joaquinpenafiel/ai-api-observability)
- [Architecture & Engineering Decisions](https://github.com/joaquinpenafiel/ai-api-observability/blob/main/docs/ARCHITECTURE.md)
- [API Documentation](https://ai-api-observability-production.up.railway.app/docs)

Direct Gemini and Anthropic HTTP integrations, retries with exponential
backoff, request tracing, HMAC-SHA256 signed webhooks, SQL-backed telemetry,
token and cost tracking, Docker, CI and 38 automated tests.

A dedicated load probe separated HTTP-layer degradation from SQLite write
contention. Controlled follow-up experiments showed that WAL mode combined with
persistent worker-local connections moved the measured persistence boundary
substantially — roughly 3.7x to 4.4x more successful-write throughput across the
tested concurrency range, with fewer lock errors and lower latency. The
optimisation moved the boundary; it did not remove contention at higher
concurrency.

---

### Conformal Prediction for Chaotic Three-Body Systems

Preregistered experimental program that measures **where a conformal prediction
instrument stops being useful**, and separates that boundary from the point
where it stops being valid.

**Links**

- [Repository](https://github.com/joaquinpenafiel/conformal-prediction-three-body)
- [Document index](https://github.com/joaquinpenafiel/conformal-prediction-three-body/blob/main/docs/INDEX.md)
- [Short demonstration run](https://github.com/joaquinpenafiel/conformal-prediction-three-body/tree/main/demo)

Three closed stages characterise the operating domain of the instrument. Every
stage was frozen before execution, guarded by gates that abort the run, and
closed by a mechanical verdict computed over criteria fixed in advance. The
full chain — preregistrations, minutes, amendments, code, data and outputs — is
anchored by SHA-256 and verified in ten seconds by `python verify.py`, which
runs on CI with every change.

The result: at four times the reference horizon the regions are still valid —
coverage holds within tolerance at all five nominal levels — while the geometric
regime that makes them informative is lost earlier. The characterised limit is
one of informativeness, not of validity.

What the program is worth showing for is that the machinery actually fired: a
gate aborted a run and the tolerance was amended with a value derived from the
integrator's own precision rather than from the observed discrepancy; a binding
criterion bounded the domain instead of confirming a hypothesis; a preregistered
prediction failed and is reported as failed; and cross-auditing caught a
blocking defect in every stage.

The demonstration run reproduced the published results from an unrelated machine
and software stack: coverage exact, conformal radius to 8.6e-11 relative, over
120 cells.

---

## Core technologies

**Backend:** Python, FastAPI, JavaScript/Node.js, REST APIs, httpx, Webhooks

**Data:** SQL, MySQL, SQLite, data migration, validation and normalization

**Reliability & Delivery:** pytest, structured logging, request tracing, Docker,
GitHub Actions, Railway

**Applied AI:** AI-provider integrations, token/cost telemetry, provider
normalization and failure handling

**Research engineering:** experimental design, preregistration, abort gates,
provenance and hash-anchored reproducibility, conformal prediction,
uncertainty quantification

## Professional focus

Backend Engineering • Applied AI • Research Engineering • API & Systems
Integration • Automation • Data-intensive Systems • Reliability & Observability

I value explicit engineering trade-offs, reproducible experiments and systems
whose behavior can be inspected and tested.

[LinkedIn](https://www.linkedin.com/in/joaquin-penafiel/) ·
[ORCID 0009-0005-2614-9393](https://orcid.org/0009-0005-2614-9393)
