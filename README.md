Twelve years building products and the platforms they run on. I like owning a problem end to end — the feature, the service under it, the pipeline that ships it, and the instrumentation that tells us it worked.

Lately most of my code is written by agents, driven by my specs and review. So I'm building the tooling for that.

### Now — [jig](https://github.com/ygrishajev/jig)

An agent-driven delivery loop: a Markdown request goes in, a reviewed plan, reviewed commits and a PR description come out.

- Plan → design review → implement in slices → verify and review each slice → final whole-request check
- Runs Claude Code, OpenCode or Codex unattended in a Docker sandbox ([sandcastle](https://github.com/mattpocock/sandcastle)) on a private clone; only implementation commits come back to the host
- Mix agents per role via presets (e.g. Codex reviewing OpenCode), optional design checkpoint, human merge by default
- jig builds jig: 71 of its 366 commits are authored by jig itself
- TypeScript, published on npm as [`@ygrishajev/jig`](https://www.npmjs.com/package/@ygrishajev/jig) · [architecture map](https://ygrishajev.github.io/jig/architecture.html)

### Akash Console @ Overclock Labs · Feb 2024 – Aug 2026

[**605 merged PRs**](https://github.com/akash-network/console/pulls?q=is%3Apr+author%3Aygrishajev+is%3Amerged) in the Console monorepo, plus work in `akashjs`, `akash-api` and `helm-charts`.

- Migrated services from raw GCP and manual deploys to Kubernetes, one Helm chart per service
- Built the observability stack: OpenTelemetry, Grafana, Prometheus, Loki, alerting
- Monorepo and release automation behind a move from 2 → 10 independently deployable services; deploy frequency ~45 → ~170 releases/month
- Billing and managed-wallet platform: Stripe checkout, custodial wallets, automated top-ups, fee grants, batch transaction signing
- Alerting and notifications pipeline, feature flags (Unleash), secrets management (Doppler), product analytics
- Shipped the Console onboarding redesign end to end with agents, from Linear scoping to implementation

### Before

**Software Engineering Team Lead** @readyplayerme — led a team of 7 and helped grow the org from 5 to 30+ engineers: one of several technical interviewers through that growth, plus onboarding and team structure. Built the internal microservices platform — core libraries, service templates, shared CI — behind an avatar API used by 3,500+ developers. Team owned Studio, the developer dashboard: Asset Manager, Asset Designer, per-app theming.

**Lead Engineer** @PeakersInc — personalization engine, payments and subscriptions, realtime chat over GraphQL subscriptions.

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

**Stack:** TypeScript · Node.js · NestJS · React / Next.js · PostgreSQL · Kubernetes · OpenTelemetry · Stripe

Open to senior / staff product and platform roles, remote · [LinkedIn](https://linkedin.com/in/igryshaiev)
