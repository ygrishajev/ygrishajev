# Iaroslav Gryshaiev

Platform and full-stack engineer. TypeScript, Node.js, Kubernetes, PostgreSQL.

I build the internal platform — release automation, observability, developer tooling — and ship product on top of it.

### Now — Akash Console @ Overclock Labs

[**660 merged PRs**](https://github.com/search?q=org%3Aakash-network+author%3Aygrishajev+is%3Apr+is%3Amerged&type=pullrequests) across the `akash-network` org since Feb 2024.

- Migrated services from raw GCP and manual deploys to Kubernetes, one Helm chart per service
- Built the observability stack: OpenTelemetry, Grafana, Prometheus, Loki, alerting
- Monorepo and release automation behind a move from 2 → 10 independently deployable services; deploy frequency ~45 → ~170 releases/month
- Payments and managed-wallet platform: Stripe checkout, custodial wallets, automated top-ups, fee grants, batch transaction signing
- Took three services from first commit to production: log forwarding, notifications, transaction signing

### Before

**Software Engineering Team Lead** @ Ready Player Me — led a team of 7 inside an org that grew from 5 to 30+ engineers; built the internal microservices platform (core libraries, service templates, shared CI) behind an avatar API used by 3,500+ developers.

**Lead Engineer** @ Peakers — personalization engine, monolith → event-driven microservices.

### A few PRs worth reading

- [Replacing a distributed lock with idempotency](https://github.com/akash-network/console/pull/2720) — removed Postgres advisory-lock coordination after auditing every critical section it guarded; unblocked horizontal scaling of the API
- [Tuning the database connection pool](https://github.com/akash-network/console/pull/2795) — diagnosed cold-connection churn with OpenTelemetry span metrics rather than guesswork
- [Making the job queue's pool configurable](https://github.com/akash-network/console/pull/2823) — the actual fix for pod restarts: a shared queue starving the request path

---

📍 Spain · remote
[LinkedIn](https://www.linkedin.com/in/iaroslav-gryshaiev-a4172045)
