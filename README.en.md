# Kotaro Minamiyama 👋

<div align="right">
  <a href="README.md">日本語</a> | <strong>English</strong>
</div>

### Lead Architect & High-Performance Full-Stack Engineer

> **Specializing in "Zero-to-One Microservices" × "Low-Level OSS Tooling" × "High-Load Enterprise Resiliency" × "Legacy Structural Debt & Security Diagnosis"**  
> An engineer who goes beyond simply making code "work"—dedicated to enforcing strict security, computational efficiency, low coupling, clear separation of concerns, and robust governance for sustainable, high-reliability architectures.

---

## 🎯 Engineering Philosophy & Principles

| Principle / Value | Practice & Architectural Mindset |
| :--- | :--- |
| **🛡️ Security & Governance First** | Never settle for "it just works in production." Ensure uncompromising security across authentication/authorization, dependency vulnerabilities (Supply Chain Security), encryption, and comprehensive audit logs. |
| **⚡ High Performance & Low Latency** | Maximize computational and query efficiency, minimize memory footprint, and leverage Rust / Java 25 high concurrency and zero-copy parsing for low-cost, ultra-low-latency foundations. |
| **🧩 Clear Separation of Concerns & Low Coupling** | Strictly define boundaries and responsibilities across frontend (BFF), backend services, and microservices. Ruthlessly eliminate inverse dependencies and tight coupling. |
| **📊 Quantitative Debt Management & Observability** | Quantitatively illuminate and resolve hidden architectural debt and performance bottlenecks via OpenTelemetry/Grafana observability, static dependency analysis, and load testing (k6/JMeter). |

---

## ⚡ Core Strengths & Expertise

### 1. 🚀 Ultra-Fast Microservices & Modern Full-Stack (Rust / Next.js / gRPC)
- **12 Core Microservices Architecture**: Engineered a complete multi-tenant SaaS from scratch using **Rust (Axum / Tonic / gRPC) + dedicated scheduler + batch processing + Neo4j (Graph DB) + Next.js (App Router) Monorepo**.
- **High Concurrency & Low Latency**: Proven via k6 load testing — **150–160 concurrent VUs, 0% error rate, p95 latency < 600ms**.
- **Full-Cycle Observability**: Deployed production-grade distributed tracing and telemetry using **OpenTelemetry + Grafana OSS (Prometheus, Loki, Tempo)**.

### 2. 🦀 Low-Level Systems & High-Performance Parsers / Tooling (Rust OSS)
- **[`xlsxparser`](https://github.com/MinamiyamaKotaro/xlsxparser)**: Ultra-lightweight, high-performance `.xlsx` (OOXML) streaming parser in Rust. Specifically engineered to handle massive spreadsheets, complex merged cells, and irregular layouts with minimal memory footprint.
- **`exceldiff` / [`extmd`](https://github.com/MinamiyamaKotaro/extmd)**: High-precision Excel diff engine & Markdown conversion CLI with layout overflow detection. Eliminates data degradation in tabular versioning and automates CI workflows.

### 3. ☕ Enterprise Backend & High-Load Performance Tuning (Java 8–25)
- **10+ Years Enterprise Java**: Deep mastery spanning from legacy enterprise systems (Struts/Seasar2) to modern **Spring Boot** and the latest **Java 25**.
- **Performance & Load Testing**: Led end-to-end load testing with **JMeter / k6**, database query tuning (PostgreSQL / Oracle / MySQL), and connection pool optimization across mission-critical systems.

### 4. 🔍 Architectural Debt & Security Vulnerability Diagnosis
- **Static Dependency Analysis**: Evaluated 4,000+ file scale legacy systems (PHP/Vue/Slim), quantitatively identifying module coupling, inverse dependencies, and architectural bottlenecks.
- **Security & Governance Audits**: Executed dependency vulnerability audits (Composer/npm) and authentication flow hardening. Formulated phased short/mid/long-term refactoring roadmaps to ensure long-term maintainability.

### 5. 🛠️ True End-to-End Delivery & Troubleshooting
- **Full Lifecycle Mastery**: Requirements definition, domain modeling, DB schema design, BFF, CI/CD pipelines, container orchestration (Docker/OCI/AWS), and production monitoring.
- **Build & Cache Optimization**: Achieved **86%–90% build cache hit rate** via **sccache (Redis)** integration.
- **Critical Recovery**: Resolved over 300 integration test defects within one month, leading projects to on-time delivery as a technical lead.

---

## 💻 Tech Stack

### Languages & Runtimes
![Rust](https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white)
![Java](https://img.shields.io/badge/Java%208--25-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)

### Frameworks & Libraries
![Axum](https://img.shields.io/badge/Axum-000000?style=for-the-badge&logo=rust&logoColor=white)
![Tonic gRPC](https://img.shields.io/badge/Tonic%20(gRPC)-244f5a?style=for-the-badge&logo=grpc&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js%20(App%20Router)-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white)
![Vue.js](https://img.shields.io/badge/Vue.js%203-4FC08D?style=for-the-badge&logo=vuedotjs&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)

### Database & Storage & Middleware
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL%20%2F%20MariaDB-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Oracle DB](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white)
![Neo4j](https://img.shields.io/badge/Neo4j-008CC1?style=for-the-badge&logo=neo4j&logoColor=white)
![Redis](https://img.shields.io/badge/Redis%20Streams-DC382D?style=for-the-badge&logo=redis&logoColor=white)
![Keycloak](https://img.shields.io/badge/Keycloak-4D4D4D?style=for-the-badge&logo=keycloak&logoColor=white)

### Infra, DevOps & Observability
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![OCI](https://img.shields.io/badge/Oracle%20Cloud-F80000?style=for-the-badge&logo=oracle&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000?style=for-the-badge&logo=opentelemetry&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana%20(Prometheus%2FLoki%2FTempo)-F46800?style=for-the-badge&logo=grafana&logoColor=white)
![k6](https://img.shields.io/badge/k6%20%2F%20JMeter-7D64FF?style=for-the-badge&logo=k6&logoColor=white)


