<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/header-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/header-light.svg">
  <img alt="Rafael Pissardo — Senior Rails, Product, Reliability" src="assets/header-dark.svg" width="100%">
</picture>

<p align="center">
  <strong>Senior Rails & Product Engineer</strong><br/>
  Gems, APIs, and apps for production Rails systems.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/location-Europe%20%2F%20Remote-21262D?style=flat-square&logo=googlemaps&logoColor=white" alt="Europe / Remote"/>
  <img src="https://img.shields.io/badge/focus-Rails%208%20%C2%B7%20Solid%20Queue%20%C2%B7%20APIs-21262D?style=flat-square&logo=rubyonrails&logoColor=white" alt="Rails 8, Solid Queue, APIs"/>
</p>

<p align="center">
  <a href="https://linkedin.com/in/rafael-augusto-pissardo"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="mailto:rpissardo@hotmail.com"><img src="https://img.shields.io/badge/Email-21262D?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://rubygems.org/gems/solid_queue_guard"><img src="https://img.shields.io/badge/RubyGems-solid__queue__guard-CC342D?style=for-the-badge&logo=ruby&logoColor=white" alt="RubyGems"/></a>
</p>

---

## Gems

### [solid_queue_guard](https://github.com/rafael-pissardo/solid_queue_guard)

Production readiness checks and runtime guards for [Solid Queue](https://github.com/rails/solid_queue).

Detects queue lag, dead workers, unsafe pool config, and broken recurring jobs — before they become incidents.

| | |
|---|---|
| **RubyGems** | [solid_queue_guard](https://rubygems.org/gems/solid_queue_guard) |
| **Latest** | [![Gem Version](https://img.shields.io/gem/v/solid_queue_guard?style=flat-square)](https://rubygems.org/gems/solid_queue_guard) |
| **Downloads** | [![Downloads](https://img.shields.io/gem/dt/solid_queue_guard?style=flat-square)](https://rubygems.org/gems/solid_queue_guard) |
| **Stack** | Ruby 3.1+ · Rails 7.1–8 · Mission Control integration |

```bash
bundle add solid_queue_guard
```

---

## Apps

### [WakupCall](https://github.com/rafael-pissardo/wakupcall-api) — social alarms with sealed voice surprises

Someone records a voice message, schedules delivery, and the recipient sees **who** and **when** — never the audio — until the alarm fires. Declining is silent for the sender.

| | [API](https://github.com/rafael-pissardo/wakupcall-api) | [Android](https://github.com/rafael-pissardo/wakupcall-android) |
|---|---|---|
| **Stack** | Rails 8 · Ruby 3.4 · PostgreSQL · JWT · FCM | Kotlin · Jetpack Compose · Room |
| **Highlights** | Sealed audio · silent decline · Pundit · offline `/sync` | Exact alarms · home widget · offline-first sync |
| **Links** | Railway · GitHub Actions | [Download APK](https://github.com/rafael-pissardo/wakupcall-android/releases/latest/download/wakupcall.apk) |

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

### [Bluetile](https://github.com/rafael-pissardo/Bluetile) — user integrity check API

Real-time integrity scoring for mobile users: country whitelist, device trust, and VPN/Tor detection in a hardened Rails 8 endpoint.

| | |
|---|---|
| **Stack** | Rails 8.1 · Ruby 3.4 · PostgreSQL · Redis |
| **Highlights** | Deterministic check chain · API key auth · rate limiting · fail-open external calls · audit logging |

---

## Featured repos

| Repository | Type | What it is |
|------------|------|------------|
| [**solid_queue_guard**](https://github.com/rafael-pissardo/solid_queue_guard) | Gem | Production doctor for Solid Queue |
| [**wakupcall-api**](https://github.com/rafael-pissardo/wakupcall-api) | App | Rails backend for sealed social alarms |
| [**wakupcall-android**](https://github.com/rafael-pissardo/wakupcall-android) | App | Kotlin client — Compose, offline sync, exact alarms |
| [**Bluetile**](https://github.com/rafael-pissardo/Bluetile) | App | Rails API for real-time user integrity checks |

---

## Stack

<p>
  <img src="https://img.shields.io/badge/Ruby_on_Rails-8-D30001?style=flat-square&logo=rubyonrails&logoColor=white" alt="Rails"/>
  <img src="https://img.shields.io/badge/Ruby-3.4-CC342D?style=flat-square&logo=ruby&logoColor=white" alt="Ruby"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/Solid_Queue-21262D?style=flat-square&logo=sidekiq&logoColor=white" alt="Solid Queue"/>
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis"/>
  <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white" alt="Kotlin"/>
  <img src="https://img.shields.io/badge/Jetpack_Compose-4285F4?style=flat-square&logo=jetpackcompose&logoColor=white" alt="Compose"/>
  <img src="https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions"/>
</p>

---

## Contact

| | |
|---|---|
| **LinkedIn** | [linkedin.com/in/rafael-augusto-pissardo](https://linkedin.com/in/rafael-augusto-pissardo) |
| **Email** | [rpissardo@hotmail.com](mailto:rpissardo@hotmail.com) |
| **GitHub** | [@rafael-pissardo](https://github.com/rafael-pissardo) |
| **RubyGems** | [solid_queue_guard](https://rubygems.org/gems/solid_queue_guard) |
| **Availability** | Remote · Europe · International B2B & contract |
