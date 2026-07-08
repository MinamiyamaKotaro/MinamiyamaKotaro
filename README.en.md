# Hi there, I'm Kotaro Minamiyama 👋

I design and build microservices platforms for multi-tenant SaaS, across both backend and frontend.

## 🔭 About Me

- 🏗️ Designing and building a multi-tenant OMO (Online Merges with Offline) platform
- 🦀 Driving the migration of a Java-centric backend to Rust (Axum / tonic)
- 🔍 Focused on finding and fixing security/reliability bugs through hands-on verification

## 🧑‍💻 Skills

**Backend**
- Java
- Rust (Axum, tonic / gRPC)

**Frontend**
- TypeScript
- Next.js / Node.js

**Data**
- Neo4j

**Infra / Observability**
- Docker
- Prometheus
- OpenTelemetry

**Auth**
- Keycloak
- JWT

## 🚀 Projects

### EXI
A multi-tenant OMO platform that unifies POS, mobile ordering, inventory management, and shift scheduling (personal project, private repository).

- Rewrote the API gateway from Java to Rust (Axum), adding OpenTelemetry tracing and Prometheus metrics
- Designed the requirements and detailed design for migrating the accounting service to Rust (tonic)
- Fixed bugs found during live testing, including a missing JWT audience check and a tenant ID propagation gap in downstream gRPC calls
- Implemented per-route, per-method rate limiting
- Handled a major Next.js version upgrade and set up the frontend test infrastructure

## 📊 GitHub Stats

<p>
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=MinamiyamaKotaro&show_icons=true&theme=default" alt="Kotaro Minamiyama's GitHub stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MinamiyamaKotaro&layout=compact&theme=default" alt="Top languages" />
</p>

<p>
  <img src="https://github-profile-trophy.vercel.app/?username=MinamiyamaKotaro&theme=flat&no-frame=true&row=1" alt="GitHub trophies" />
</p>
