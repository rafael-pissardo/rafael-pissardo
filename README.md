<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/header-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/header-light.svg">
  <img alt="Rafael Pissardo — Senior Rails, Product, Reliability" src="assets/header-dark.svg" width="100%">
</picture>

<p align="center">
  <strong>Senior Rails & Product Engineer</strong><br/>
  I help teams ship business-critical software — modernize Rails systems, stabilize background jobs, and keep delivery moving.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/location-Europe%20%2F%20Remote-21262D?style=flat-square&logo=googlemaps&logoColor=white" alt="Europe / Remote"/>
  <img src="https://img.shields.io/badge/open%20to-international%20B2B%20%26%20contract-21262D?style=flat-square&logo=handshake&logoColor=white" alt="Open to international B2B and contract"/>
  <img src="https://img.shields.io/badge/focus-Rails%208%20%C2%B7%20Solid%20Queue%20%C2%B7%20Observability-21262D?style=flat-square&logo=rubyonrails&logoColor=white" alt="Rails 8, Solid Queue, Observability"/>
</p>

<p align="center">
  <a href="https://linkedin.com/in/rafael-augusto-pissardo"><img src="https://img.shields.io/badge/LinkedIn-connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:rpissardo@hotmail.com"><img src="https://img.shields.io/badge/email-rpissardo%40hotmail.com-21262D?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://github.com/rafael-pissardo/wakupcall-api"><img src="https://img.shields.io/badge/signature%20work-WakupCall-3FB950?style=for-the-badge&logo=ruby&logoColor=white" alt="WakupCall"/></a>
</p>

---

## Current focus

Building and operating **Rails backends** where product decisions, reliability, and architecture intersect.

| Area | What I'm working on |
|------|---------------------|
| **Rails modernization** | Rails 8, Solid Queue, cleaner Active Job boundaries |
| **Background jobs** | Sidekiq → Solid Queue migrations, queue observability, failure recovery |
| **Reliability** | Datadog, incident prevention, systems that stay boring under load |
| **Product engineering** | End-to-end ownership from API design to shipped user outcomes |
| **AI-assisted workflows** | Faster delivery with stronger review, testing, and documentation discipline |

> I work best where product, reliability, and backend architecture meet.

---

## Technical strengths

| Strength | Proof in practice |
|----------|-------------------|
| **Rails backend architecture** | Production APIs with auth, authorization, rate limiting, and mobile-first sync |
| **Job processing at scale** | Active Job, Solid Queue, Sidekiq migration patterns, operational dashboards |
| **Data & persistence** | PostgreSQL schema design, transactional workflows, offline sync contracts |
| **Observability & ops** | Metrics, tracing, actionable alerts — fewer surprises in production |
| **Product-minded delivery** | Full-stack product builds spanning API, mobile client, CI/CD, and deployment |
| **Remote collaboration** | Async-friendly docs, clear PRs, maintainable systems for distributed teams |

---

## Signature work

### [WakupCall](https://github.com/rafael-pissardo/wakupcall-api) — social alarms with sealed voice surprises

A product I designed and built end-to-end: **Rails API + Android client**, from domain modeling to production deployment.

Someone records a voice message, schedules delivery, and the recipient sees **who** and **when** — never the audio — until the alarm fires. Declining is **silent** for the sender.

<table>
<tr>
<th><a href="https://github.com/rafael-pissardo/wakupcall-api">API</a></th>
<th><a href="https://github.com/rafael-pissardo/wakupcall-android">Android</a></th>
</tr>
<tr>
<td>

Rails 8 · Ruby 3.4 · PostgreSQL · JWT · FCM

Sealed audio · silent decline · Pundit · Rack::Attack · offline `/sync`

Railway · GitHub Actions CI

</td>
<td>

Kotlin · Jetpack Compose · Material 3 · Room

Exact alarms · home widget · offline-first sync · Paparazzi snapshots

<a href="https://github.com/rafael-pissardo/wakupcall-android/releases/latest/download/wakupcall.apk">Download APK</a>

</td>
</tr>
</table>

```mermaid
sequenceDiagram
  participant Sender
  participant API
  participant Recipient
  Sender->>API: record + schedule surprise
  API->>Recipient: push (metadata only)
  Recipient->>API: accept or silent decline
  API->>Recipient: alarm rings with sealed audio
```

**Why it matters:** domain-driven API design, privacy-sensitive media handling, mobile sync contracts, and production-ready Rails patterns — not a tutorial app.

---

## Featured repositories

| Repository | Role | Stack |
|------------|------|-------|
| [**wakupcall-api**](https://github.com/rafael-pissardo/wakupcall-api) | Production Rails backend — auth, alarms, sealed delivery, push | Rails 8 · PostgreSQL · JWT · FCM |
| [**wakupcall-android**](https://github.com/rafael-pissardo/wakupcall-android) | Android client — Compose UI, offline sync, exact alarms | Kotlin · Compose · Room |
| [**rafael-pissardo**](https://github.com/rafael-pissardo/rafael-pissardo) | Profile, positioning, and public engineering notes | Markdown · GitHub Profile |

**Coming soon** *(repos in progress — see [execution plan](GITHUB_PROFILE_STRATEGY.md))*:

| Planned repo | Purpose |
|--------------|---------|
| `rails-job-migration-playbook` | Sidekiq → Solid Queue migration notes, checklists, and trade-offs |
| `rails-observability-kit` | Datadog + Rails patterns for metrics, traces, and alert hygiene |
| `ai-rails-engineering` | Practical AI-assisted Rails workflows with review guardrails |

---

## Tech stack

<p>
  <img src="https://img.shields.io/badge/Ruby_on_Rails-8-D30001?style=flat-square&logo=rubyonrails&logoColor=white" alt="Rails"/>
  <img src="https://img.shields.io/badge/Ruby-3.4-CC342D?style=flat-square&logo=ruby&logoColor=white" alt="Ruby"/>
  <img src="https://img.shields.io/badge/PostgreSQL-16-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis"/>
  <img src="https://img.shields.io/badge/Solid_Queue-Active_Job-21262D?style=flat-square&logo=sidekiq&logoColor=white" alt="Solid Queue"/>
  <img src="https://img.shields.io/badge/Sidekiq-migration-21262D?style=flat-square&logo=sidekiq&logoColor=white" alt="Sidekiq"/>
  <img src="https://img.shields.io/badge/AWS-ECS%20%2F%20Fargate-232F3E?style=flat-square&logo=amazonaws&logoColor=white" alt="AWS"/>
  <img src="https://img.shields.io/badge/Heroku-430098?style=flat-square&logo=heroku&logoColor=white" alt="Heroku"/>
  <img src="https://img.shields.io/badge/Datadog-632CA6?style=flat-square&logo=datadog&logoColor=white" alt="Datadog"/>
  <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white" alt="Kotlin"/>
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions"/>
</p>

---

## Writing & experiments

Documenting patterns I use in production — focused on **maintainable Rails systems**, not hype.

| Topic | Status |
|-------|--------|
| Solid Queue adoption & Sidekiq migration checklists | drafting |
| Rails observability: metrics that prevent incidents | planned |
| AI-assisted engineering with senior review discipline | planned |
| Product API design for mobile offline sync | live in WakupCall repos |

---

## Contact

| | |
|---|---|
| **LinkedIn** | [linkedin.com/in/rafael-augusto-pissardo](https://linkedin.com/in/rafael-augusto-pissardo) |
| **Email** | [rpissardo@hotmail.com](mailto:rpissardo@hotmail.com) |
| **GitHub** | [@rafael-pissardo](https://github.com/rafael-pissardo) |
| **Availability** | Remote · Europe timezone · International B2B & contract |

If you're building a Rails product, migrating background jobs, or need a senior engineer who owns outcomes — let's talk.
