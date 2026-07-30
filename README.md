# Iaroslav Gryshaiev

Platform and full-stack engineer. TypeScript, Node.js, Kubernetes, PostgreSQL.

Ten years building products and the platforms they run on. I like owning a problem end to end — the feature, the service under it, the pipeline that ships it, and the instrumentation that tells us it worked.

### Now — Akash Console @ Overclock Labs

[**590 merged PRs**](https://github.com/akash-network/console/pulls?q=is%3Apr+author%3Aygrishajev+is%3Amerged) in the Console monorepo since Feb 2024, plus work in `akashjs`, `akash-api` and `helm-charts`.

- Migrated services from raw GCP and manual deploys to Kubernetes, one Helm chart per service
- Built the observability stack: OpenTelemetry, Grafana, Prometheus, Loki, alerting
- Monorepo and release automation behind a move from 2 → 10 independently deployable services; deploy frequency ~45 → ~170 releases/month
- Payments and managed-wallet platform: Stripe checkout, custodial wallets, automated top-ups, fee grants, batch transaction signing
- Restructured the codebase into npm workspaces; created the notifications and log-forwarding services and extracted transaction signing into its own

### Before

**Software Engineering Team Lead** @ Ready Player Me — led a team of 7 inside an org that grew from 5 to 30+ engineers; built the internal microservices platform (core libraries, service templates, shared CI) behind an avatar API used by 3,500+ developers.

**Lead Engineer** @ Peakers — personalization engine, monolith → event-driven microservices.

### Things I started

In [`akash-network/console`](https://github.com/akash-network/console), where the first commit is mine:

**Services**
- [`apps/notifications`](https://github.com/akash-network/console/tree/main/apps/notifications) — alerting and notification service, built from scratch · Mar 2025
- [`apps/log-collector`](https://github.com/akash-network/console/tree/main/apps/log-collector) — log forwarding for deployments, built from scratch · Jul 2025
- [`apps/tx-signer`](https://github.com/akash-network/console/tree/main/apps/tx-signer) — transaction signing, extracted out of the API into its own service · Jan 2026

**Platform packages** — the release and developer-experience toolchain
- [`packages/releaser`](https://github.com/akash-network/console/tree/main/packages/releaser) — release with image build
- [`packages/docker`](https://github.com/akash-network/console/tree/main/packages/docker) — shared Docker setup
- [`packages/dev-config`](https://github.com/akash-network/console/tree/main/packages/dev-config) — centralized code style and TS config
- [`packages/env-loader`](https://github.com/akash-network/console/tree/main/packages/env-loader) — unified env loading

Also the npm workspaces restructuring the monorepo runs on, and sustained work across the API, web app, payments and wallet platform, provider marketplace, and the observability stack.

---

📍 Spain · remote
[LinkedIn](https://www.linkedin.com/in/iaroslav-gryshaiev-a4172045)
