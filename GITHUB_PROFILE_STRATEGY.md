# GitHub Profile Strategy — Rafael Pissardo

> **Profile analyzed:** [github.com/rafael-pissardo](https://github.com/rafael-pissardo)  
> **Note:** `github.com/rpissardo` does not exist. Your active handle is **`rafael-pissardo`**.

---

## Executive summary

**Current state:** Good foundation (WakupCall is strong proof), but the profile undersells seniority and has credibility risks from pinned third-party Rails repos and a stats widget.

**Target reaction (10 seconds):** *"Senior Rails/product engineer. Ships real products. Understands reliability and background jobs. Worth a conversation."*

**Priority fixes:**
1. Replace pinned repos (remove upstream `jets`, `solid_queue`, `mission_control-jobs`)
2. Publish new profile README (done in this repo)
3. Update GitHub bio + display name
4. Create 3 showcase repos for Rails reliability / jobs / AI workflows
5. Archive or hide low-signal repos

---

## 1. Brand positioning

Three positioning statements (pick one for bio; rotate in LinkedIn):

| # | Statement |
|---|-----------|
| **A (recommended)** | Senior Rails engineer modernizing production systems without slowing delivery. |
| **B** | Product-minded backend engineer — Rails, reliability, and systems that stay maintainable under pressure. |
| **C** | I help Rails teams ship business-critical software with strong ownership across architecture, jobs, and ops. |

**Bio (GitHub — 160 chars max):**
```
Senior Rails & product engineer. Rails 8, Solid Queue, observability, AI-assisted delivery. Remote · Europe · B2B/contract.
```

---

## 2. Visual concept

| Element | Direction |
|---------|-----------|
| **Color palette** | `#0D1117` base · `#3FB950` accent · `#58A6FF` links · `#8B949E` muted · `#D30001` Rails |
| **Typography feel** | System sans-serif, strong hierarchy, short lines — no decorative fonts |
| **Badge style** | shields.io `flat-square` for stack; `for-the-badge` only for CTAs (max 3 in hero) |
| **Header** | SVG banner with dark/light variants via `<picture>` |
| **Emoji policy** | None in hero; zero in section headers; contact table stays clean |
| **Icon policy** | Logo badges only (Rails, PostgreSQL, AWS, Datadog) — no icon walls |
| **Visual density** | Medium-low: one case study, one diagram, one stack row |
| **Dark/light** | SVG header swaps; badge colors work on both GitHub themes |

**Avoid:** snake animation, streak stats, trophy badges, rainbow gradients, meme headers.

---

## 3. Profile README structure

| Section | Purpose | Treatment | Avoid |
|---------|---------|-----------|-------|
| **Hero** | Identity + CTA in 5 seconds | SVG banner + role + 3 CTAs | "Passionate developer", emoji spam |
| **One-line positioning** | Subtitle under name | Single sentence, outcome-focused | Buzzword lists |
| **Current focus** | What you're doing now | Compact table | Vague "learning X" |
| **Technical strengths** | Seniority signals | Proof-oriented table | Adjectives without evidence |
| **Signature work** | Deepest proof | WakupCall case study + mermaid | Too many projects |
| **Featured repos** | Navigation to code | 3 live + 3 planned | Forks you didn't build |
| **Tech stack** | Recruiter scan | One badge row | 30+ badges |
| **Writing / experiments** | Thought leadership | Honest status table | Empty blog links |
| **Contact** | Conversion | Table + availability | Only social icons |

---

## 4. Hero section (implemented)

See [`README.md`](README.md) — includes:
- Name + role
- Positioning phrase
- Remote / B2B availability
- Stack focus badges
- LinkedIn · Email · WakupCall CTAs

---

## 5. Pinned repository strategy

### Unpin immediately (credibility risk)

| Repo | Problem |
|------|---------|
| `rubyonjets/jets` | Not your project — implies false ownership |
| `rails/solid_queue` | Upstream project, not your contribution showcase |
| `rails/mission_control-jobs` | Same as above |

### Pin these 6 (in order)

| # | Repo | Status | Purpose | README angle |
|---|------|--------|---------|--------------|
| 1 | **wakupcall-api** | ✅ exists | Serious Rails product app | Production API: sealed media, auth, sync, CI/CD |
| 2 | **wakupcall-android** | ✅ exists | Full product story | Mobile client proving end-to-end ownership |
| 3 | **rails-job-migration-playbook** | 🔨 create | Sidekiq → Solid Queue | Checklists, cutover runbooks, rollback, metrics |
| 4 | **rails-observability-kit** | 🔨 create | Reliability / Datadog | Rails + Datadog patterns, alert hygiene, dashboards |
| 5 | **ai-rails-engineering** | 🔨 create | AI-assisted workflows | Prompts, review gates, test generation guardrails |
| 6 | **rafael-pissardo** | ✅ exists | Portfolio / positioning | This profile README + public notes |

### Per-repo recommendations

#### wakupcall-api
- **Why it matters:** Real Rails 8 product with non-trivial domain (sealed audio, silent decline)
- **Badges:** CI, Railway, Rails 8, Ruby, PostgreSQL *(already good)*
- **First impression:** Add architecture diagram + "Key decisions" section

#### wakupcall-android
- **Why it matters:** Proves product ownership beyond backend
- **Badges:** CI, APK download, Kotlin, Compose *(already good)*
- **First impression:** Add 2–3 screenshots in README

#### rails-job-migration-playbook *(to create)*
- **Purpose:** Document Sidekiq → Solid Queue migration with trade-offs
- **README angle:** Problem → approach → checklist → rollback → observability
- **Badges:** Rails, Solid Queue, Sidekiq, PostgreSQL

#### rails-observability-kit *(to create)*
- **Purpose:** Datadog + Rails reference patterns
- **README angle:** Metrics, traces, logs, SLO-friendly alerts
- **Badges:** Rails, Datadog, AWS

#### ai-rails-engineering *(to create)*
- **Purpose:** AI-assisted development with senior review discipline
- **README angle:** Workflows, not hype — spec → implement → verify
- **Badges:** Rails, Ruby, GitHub Actions

#### rafael-pissardo
- **Purpose:** Profile hub and case-study index
- **README angle:** Already implemented

---

## 6. Repository README checklist

Apply to **wakupcall-api**, **wakupcall-android**, and each new repo:

- [ ] Clear problem statement (1 paragraph)
- [ ] Architecture diagram or screenshots
- [ ] Setup instructions (Docker + native)
- [ ] Tech stack badges (consistent style)
- [ ] Key decisions (3–5 bullets)
- [ ] Trade-offs (what you chose vs. alternatives)
- [ ] Tests (how to run, coverage approach)
- [ ] Deployment info (Railway / AWS / Heroku)
- [ ] Demo link when available
- [ ] **What I would improve next** (shows senior judgment)

---

## 7. Hype elements with taste

| Element | Verdict | Implementation |
|---------|---------|----------------|
| SVG banner | ✅ Yes | `assets/header-dark.svg` + light variant |
| shields.io badges | ✅ Yes | flat-square, limited count |
| Mermaid diagram | ✅ Yes | WakupCall flow (already strong) |
| GitHub stats widget | ❌ No | Low signal at 8 public repos; feels junior |
| Contribution snake | ❌ No | Off-brand |
| Streak stats | ❌ No | Noise |
| Case-study cards | ✅ Yes | Table format in README |
| "Currently building" | ✅ Yes | Current focus table |
| Architecture diagrams | ✅ Yes | Add to WakupCall API README |
| Product screenshots | ✅ Yes | Add to Android README |

---

## 8. Content rules (applied)

- English throughout
- Confident, humble tone
- Concrete proof over adjectives
- Business + technical impact where possible
- No "passionate", "coding since forever", "always learning"
- Short sections, scannable tables

---

## 9. Rafael-specific messaging

Themes prioritized in README:
- Rails modernization (Rails 8)
- Backend architecture
- Job processing (Solid Queue / Sidekiq)
- Observability & incident prevention
- AI-assisted engineering workflows
- Product-minded delivery
- Remote international B2B readiness
- Maintainable systems under pressure

---

## 10. Account cleanup checklist

### Profile settings
- [ ] Display name: **Rafael Pissardo** (not "Pissardo")
- [ ] Bio: use recommended text above
- [ ] Location: `Europe · Remote` (or keep Vera, Spain + Remote)
- [ ] Website: LinkedIn URL
- [ ] Pronouns: optional
- [ ] Enable **Available for hire** if open to contract/B2B

### Repositories
- [ ] Unpin `jets`, `solid_queue`, `mission_control-jobs`
- [ ] Pin 6 repos per strategy above
- [ ] Archive or delete `github-readme-stats` fork (low signal)
- [ ] Archive or rename `Revelo-9011` (unclear purpose publicly)
- [ ] Archive `docs` (Mintlify starter — or repurpose for engineering notes)
- [ ] Delete unused forks: `solid_queue`, `mission_control-jobs` if no contributions planned

### README quality
- [x] Profile README rewritten
- [ ] Add architecture diagram to wakupcall-api
- [ ] Add screenshots to wakupcall-android
- [ ] Create 3 planned showcase repos

---

## 11. Missing assets to create

| Asset | Priority | Notes |
|-------|----------|-------|
| Profile SVG banners | ✅ Done | `assets/header-*.svg` |
| WakupCall API architecture diagram | High | Mermaid or PNG in repo |
| WakupCall Android screenshots (3) | High | Onboarding, alarm, surprise replay |
| `rails-job-migration-playbook` repo | High | Even a solid README + checklist adds credibility |
| `rails-observability-kit` repo | Medium | Datadog + Rails examples |
| `ai-rails-engineering` repo | Medium | Workflow docs, not prompt dumps |
| LinkedIn headline aligned with positioning | High | Match GitHub bio |

---

## 12. Seven-day execution plan

| Day | Task | Done when |
|-----|------|-----------|
| **Day 1** | Publish profile README + SVG banners; update bio & display name | Profile looks senior at first glance |
| **Day 2** | Fix pinned repos (unpin upstream, pin WakupCall + profile) | Pins show *your* work only |
| **Day 3** | WakupCall API README: add architecture diagram + "Key decisions" + "What's next" | Repo tells a senior story |
| **Day 4** | WakupCall Android README: add 3 screenshots + release badge polish | Visual proof of product |
| **Day 5** | Create `rails-job-migration-playbook` with Sidekiq → Solid Queue checklist | Pin slot #3 filled |
| **Day 6** | Create `rails-observability-kit` starter (Datadog patterns) | Pin slot #4 filled |
| **Day 7** | Create `ai-rails-engineering`; archive/delete low-signal repos; LinkedIn sync | 6 strong pins, clean account |

---

## Review criteria — final check

| Criterion | Status |
|-----------|--------|
| Looks senior | ✅ After README + pin fix |
| Looks international | ✅ Remote · B2B · English |
| Looks credible | ⚠️ Remove misleading pins |
| Explains role in <10s | ✅ Hero + positioning |
| Strong pinned repos | ⚠️ 2/6 ready; 3 to create |
| Avoids visual noise | ✅ No stats widget |
| Shows business + technical impact | ✅ WakupCall case study |
| Recruiter/founder appeal | ✅ CTAs + contact table |
| Supports Rails/backend/product/reliability | ✅ Stack + focus sections |

---

*Generated as part of the GitHub Hype Profile Designer implementation.*
