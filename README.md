<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/header-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/header-light.svg">
  <img alt="Rafael Pissardo — Senior Backend Engineer, Ruby on Rails, Reliability" src="assets/header-dark.svg" width="100%">
</picture>

<p align="center">
  <strong>Senior Backend Engineer · Ruby on Rails · Tech Lead</strong><br/>
  Production systems, background processing, PostgreSQL and reliability.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/location-Valencia%2C%20Spain-21262D?style=flat-square&logo=googlemaps&logoColor=white" alt="Valencia, Spain"/>
  <img src="https://img.shields.io/badge/focus-Rails%208%20%C2%B7%20PostgreSQL%20%C2%B7%20Solid%20Queue-21262D?style=flat-square&logo=rubyonrails&logoColor=white" alt="Rails 8, PostgreSQL, Solid Queue"/>
</p>

<p align="center">
  <a href="https://linkedin.com/in/rafael-augusto-pissardo"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:rpissardo@gmail.com"><img src="https://img.shields.io/badge/Email-21262D?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://rubygems.org/gems/solid_queue_guard"><img src="https://img.shields.io/badge/RubyGems-solid__queue__guard-CC342D?style=for-the-badge&logo=ruby&logoColor=white" alt="RubyGems"/></a>
</p>

---

## About

I'm a **Senior Backend Engineer and hands-on Tech Lead** focused on Ruby on Rails, PostgreSQL, background processing and production reliability.

I build and operate backend systems where performance, observability and predictable failure handling matter. My work includes high-volume background job processing, Rails infrastructure, AWS deployments, database performance, CI/CD and engineering leadership.

I also contribute to the Rails ecosystem and maintain open-source tooling around Solid Queue.

---

## Rails Open Source

### Rails / Solid Queue contributor

I have **5 merged contributions** to [`rails/solid_queue`](https://github.com/rails/solid_queue), focused on production reliability, worker lifecycle, recurring jobs and test stability.

| PR | Contribution |
|---|---|
| [#770](https://github.com/rails/solid_queue/pull/770) | Honour `TERM` during supervisor boot before forking workers |
| [#768](https://github.com/rails/solid_queue/pull/768) | Stop workers when job finalization fails |
| [#758](https://github.com/rails/solid_queue/pull/758) | Reduce flaky integration failures around concurrency and lifecycle timing |
| [#757](https://github.com/rails/solid_queue/pull/757) | Add `--only-recurring` scheduler mode |
| [#756](https://github.com/rails/solid_queue/pull/756) | Report rescued recurring enqueue errors through `Rails.error` |

These contributions reflect the areas I care about most in production systems:

- predictable process lifecycle
- resilient background execution
- observable failures
- concurrency correctness
- operational simplicity
- reliable test suites

---

## Open Source

### [solid_queue_guard](https://github.com/rafael-pissardo/solid_queue_guard)

**Production diagnostics and reliability tooling for Rails applications using Solid Queue.**

It detects queue lag, dead workers, missing schedulers, unsafe database pool sizing, broken recurring jobs and other failure modes that can leave the Rails web tier healthy while background processing is not.

| | |
|---|---|
| **RubyGems** | [solid_queue_guard](https://rubygems.org/gems/solid_queue_guard) |
| **Latest** | [![Gem Version](https://img.shields.io/gem/v/solid_queue_guard?style=flat-square)](https://rubygems.org/gems/solid_queue_guard) |
| **Downloads** | [![Downloads](https://img.shields.io/gem/dt/solid_queue_guard?style=flat-square)](https://rubygems.org/gems/solid_queue_guard) |
| **Stack** | Ruby 3.1+ · Rails 7.1–8 · Solid Queue · Mission Control |

```bash
bundle add solid_queue_guard
```

### What it covers

- pre-deploy configuration checks
- queue lag detection
- stale and dead worker detection
- scheduler and recurring-job validation
- database pool sizing checks
- HTTP health endpoints
- CI deployment gates
- Mission Control integration
- Datadog metrics
- Prometheus / OpenTelemetry export

The goal is simple: detect background-processing failures **before they become production incidents**.

---

## Projects

### [WakupCall](https://github.com/rafael-pissardo/wakupcall-api)

A production-style social alarm platform with a **Rails backend and Android client**.

Someone records a voice message, schedules delivery, and the recipient sees **who** and **when** — but never hears the recording until the alarm fires.

| | [API](https://github.com/rafael-pissardo/wakupcall-api) | [Android](https://github.com/rafael-pissardo/wakupcall-android) |
|---|---|---|
| **Stack** | Rails 8 · Ruby 3.4 · PostgreSQL · Solid Queue · JWT | Kotlin · Jetpack Compose · Room |
| **Highlights** | Pundit · signed blobs · rate limiting · refresh token rotation · offline sync | Exact alarms · widgets · offline-first sync |
| **Delivery** | Railway · GitHub Actions | GitHub Releases |

The backend demonstrates:

- REST API design
- authentication and authorization
- background processing
- signed media delivery
- mobile synchronization
- security hardening
- rate limiting
- CI/CD
- production deployment

---

### [Bluetile](https://github.com/rafael-pissardo/Bluetile)

Rails API for **real-time user integrity and device trust checks**.

| | |
|---|---|
| **Stack** | Rails 8.1 · Ruby 3.4 · PostgreSQL · Redis |
| **Highlights** | Deterministic check chain · API key auth · rate limiting · VPN/Tor detection · audit logging |

Built around predictable checks, failure isolation and hardened API behavior.

---

## Featured repositories

| Repository | Type | Focus |
|---|---|---|
| [**solid_queue_guard**](https://github.com/rafael-pissardo/solid_queue_guard) | Gem | Solid Queue reliability and production diagnostics |
| [**rails/solid_queue contributions**](https://github.com/rails/solid_queue/pulls?q=is%3Apr+author%3Arafael-pissardo) | OSS | Worker lifecycle, recurring jobs and reliability |
| [**wakupcall-api**](https://github.com/rafael-pissardo/wakupcall-api) | App | Rails backend, security, jobs and mobile sync |
| [**wakupcall-android**](https://github.com/rafael-pissardo/wakupcall-android) | App | Kotlin, Compose and offline-first mobile |
| [**Bluetile**](https://github.com/rafael-pissardo/Bluetile) | App | Real-time integrity checks API |

---

## Core stack

<p>
  <img src="https://img.shields.io/badge/Ruby_on_Rails-8-D30001?style=flat-square&logo=rubyonrails&logoColor=white" alt="Rails"/>
  <img src="https://img.shields.io/badge/Ruby-3.4-CC342D?style=flat-square&logo=ruby&logoColor=white" alt="Ruby"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/Solid_Queue-21262D?style=flat-square&logo=rubyonrails&logoColor=white" alt="Solid Queue"/>
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis"/>
  <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white" alt="AWS"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker"/>
  <img src="https://img.shields.io/badge/RSpec-CC342D?style=flat-square&logo=ruby&logoColor=white" alt="RSpec"/>
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions"/>
</p>

### Engineering focus

- Backend architecture
- Ruby on Rails
- PostgreSQL performance
- Background processing
- Production reliability
- Observability
- AWS ECS / Fargate
- Docker
- CI/CD
- Automated testing
- Technical leadership
- Mentoring and code review

---

## Production experience

I have worked on Rails systems where background processing, reliability and operational visibility are core requirements.

Recent work includes:

- migration from Sidekiq to Solid Queue
- processing workloads of **2M+ background jobs**
- approximately **23% improvement in processing time**
- Rails workloads deployed on AWS ECS/Fargate
- PostgreSQL and Redis infrastructure
- Datadog observability
- production health checks and worker monitoring
- automated test suites with high coverage
- technical leadership and engineering standards

---

## How I work

I prefer engineering environments with:

- strong ownership
- pragmatic architecture
- automated testing
- small, reviewable changes
- observability from day one
- continuous delivery
- constructive code review
- engineers close to production

I enjoy staying deeply hands-on while also contributing to technical direction, architecture, mentoring and engineering standards.

---

## Contact

| | |
|---|---|
| **LinkedIn** | [linkedin.com/in/rafael-augusto-pissardo](https://linkedin.com/in/rafael-augusto-pissardo) |
| **Email** | [rpissardo@gmail.com](mailto:rpissardo@gmail.com) |
| **GitHub** | [@rafael-pissardo](https://github.com/rafael-pissardo) |
| **RubyGems** | [solid_queue_guard](https://rubygems.org/gems/solid_queue_guard) |
| **Location** | Valencia, Spain |
| **Availability** | Europe remote · International B2B · Backend / Rails / Tech Lead |

---

<p align="center">
  <strong>Building Rails systems that keep working when production gets interesting.</strong>
</p>
