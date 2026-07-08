# Kotaro Minamiyama

I design and build microservices platforms for multi-tenant SaaS, across both backend and frontend.

## Currently working on

**EXI** — a multi-tenant OMO (Online Merges with Offline) platform that unifies POS, mobile ordering, inventory management, and shift scheduling.

- Offline-capable in-store operations with real-time inventory sync
- AI-driven recommendations based on purchase history and an affinity graph (Neo4j)
- A scalable microservices architecture with per-tenant data isolation

## Recent technical work

- Rewrote the API gateway from Java to Rust (Axum), adding OpenTelemetry tracing and Prometheus metrics
- Designed the requirements and detailed design for migrating the accounting service to Rust (tonic)
- Fixed security and reliability bugs found during live testing, including a missing JWT audience check and a tenant ID propagation gap in downstream gRPC calls
- Implemented per-route, per-method rate limiting
- Handled a major Next.js version upgrade and set up the frontend test infrastructure

## Tech stack

- **Backend**: Java, Rust (Axum, tonic / gRPC)
- **Frontend**: TypeScript, Next.js, Node.js
- **Data**: Neo4j
- **Infra / Observability**: Docker, Prometheus, OpenTelemetry
- **Auth**: Keycloak, JWT
