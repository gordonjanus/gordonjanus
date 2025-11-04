# Hi 👋

Senior Software Engineer • Python • AWS • React.js

---

### TL;DR
- 8+ years designing, building, and scaling cloud-native products.
- Lead dev on data-heavy Python services and customer-facing React apps.
- Deep AWS: ECS/EKS, Lambda, API Gateway, Step Functions, SQS/SNS, DynamoDB, RDS, CDK/Terraform, CloudWatch, IAM.
- Pragmatic engineering values: small, frequent releases; strong typing/tests; observability-first.

---

## 🧰 Tech Stack

**Languages:** Python (3.10+), TypeScript/JavaScript, SQL

**Backend:** FastAPI, Django/DRF, Flask; AsyncIO; Celery; GraphQL (Ariadne/Strawberry); gRPC

**Frontend:** React 18, Next.js, Vite, Redux Toolkit/Zustand, React Query/TanStack, Tailwind CSS

**Cloud & DevOps:** AWS (ECS/EKS, Lambda, API GW, SQS/SNS, Step Functions, DynamoDB, RDS, S3, CloudFront, Route 53), Docker, Kubernetes, Terraform, AWS CDK, GitHub Actions, ArgoCD

**Data & ML:** Postgres, MySQL, Redis, OpenSearch/Elasticsearch, Pandas, NumPy; event streams (Kinesis/Kafka)

**Quality & Observability:** PyTest, Coverage, mypy, Ruff/Flake8, ESLint/Prettier, Playwright, OpenTelemetry, Prometheus + Grafana, Sentry

**Security:** IAM, KMS, Secrets Manager, Cognito, OIDC/OAuth2, OWASP, Bandit, Trivy

> Badges (optional):
>
> ![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
> ![AWS](https://img.shields.io/badge/AWS-232F3E?logo=amazon-aws&logoColor=FF9900)
> ![React](https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB)
> ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
> ![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)

---

## 🏗️ What I Build

- **Cloud-native Python services** with FastAPI, async IO, structured logging, and OpenTelemetry tracing.
- **Modern React frontends** (Next.js) with SSR/ISR, accessible UI, and testable component architecture.
- **Resilient AWS systems**—event-driven pipelines, idempotent consumers, retries/backoff, and DLQs.
- **CI/CD at scale**—trunk-based development, GitHub Actions, preview environments, automated security scans.

```text
+------------------+        +-------------+        +------------------+
|  React (Next.js) | <----> |  API GW     | <----> |  FastAPI Service |
+------------------+        +-------------+        +------------------+
         |                          |                         |
         v                          v                         v
     CloudFront                   Lambda                 DynamoDB/RDS
         |                          |                         |
         +--------------------------+-------------------------+
                            SQS/SNS / EventBridge
```

---

## 🌟 Highlights
- Cut p95 latency by **45%** moving hot paths to async FastAPI + Redis caching.
- Deployed multi-tenant SaaS on AWS (ECS + RDS + S3 + CloudFront) serving **1M+ MAU**.
- Drove test coverage from 42% → 85% with pragmatic unit/integration/e2e tests.
- Led React rewrite to Next.js 14 with app router, reducing TTFB by **~30%**.

---

## 🔧 Selected Projects

### 1) Event-Driven Data Ingestion Platform
**Stack:** Python (FastAPI), AWS Lambda, SQS/SNS, Step Functions, DynamoDB, CDK, OpenSearch

- Built idempotent ingestion & enrichment with dead-letter handling and replay.
- Structured logs (JSON), end-to-end tracing with OpenTelemetry → CloudWatch/Tempo.
- IaC with CDK (pipelines, stages, permissions least-privilege via IAM policies).
