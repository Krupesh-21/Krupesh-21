## Senior Software Engineer — Go · React · TypeScript

I build backend services in Go and ship product-quality frontends in React and TypeScript.
Systems I own stay running — I write the postmortems, fix the root causes, and close the gaps.
OSS contributions to production Go projects. End-to-end ownership: schema to deployment.

- Reduced frontend load time **5s → 3s**, bundle size by **20%**
- Improved query performance **25–30%** via caching architecture redesign
- Products serving **1,200+ DAU**

---

## At a Glance

| | |
|---|---|
| Experience | 5 years, 4 companies |
| OSS | Merged contributions to production Go projects — memory leak fix, full-stack feature |
| Products | 1,200+ DAU |
| Performance | 5s → 3s load · 20% bundle reduction · 25–30% query gains |
| Stack | Go · React · TypeScript · PostgreSQL · Redis · AWS |
| Timezone | IST — async-first with US and EU teams |

---

## Featured Work

**[TikTok Trend Analyzer](#)**
*Problem: offline support for data-heavy views.*
Stale-while-revalidate caching via service workers — instant renders from cache, fresh data in the background.

**[Gemini AI Teams Extension](#)**
*Problem: Teams DOM changes frequently, breaking injected UI.*
MutationObserver-based injection strategy with defensive selectors that degrade gracefully.

**[floatpane/matcha — Memory Leak Fix](https://github.com/floatpane/matcha)**
*Problem: unbounded sync.Map growth in production image cache.*
Replaced with LRU eviction via hashicorp/golang-lru. Merged in 24h. → *See the PR.*

**[agjmills/trove — v0.10.0](https://github.com/agjmills/trove)**
*Problem: no user-controlled sort order on file listings.*
Full-stack: Go + GORM + parameterized queries + JS frontend + test coverage. → *See the diff.*

---

## Open Source

### [floatpane/matcha](https://github.com/floatpane/matcha) — Memory Leak Fix

**Problem.** Remote image cache used an unbounded `sync.Map` — every unique URL accumulated indefinitely with no eviction and no size limit.

**Fix.** Replaced with [`hashicorp/golang-lru`](https://github.com/hashicorp/golang-lru), 20-entry cap, LRU eviction. Added tests verifying eviction behavior at capacity.

**Outcome.** Eliminated unbounded memory growth. Merged within 24 hours.

---

### [agjmills/trove](https://github.com/agjmills/trove) — Sortable File Listings (v0.10.0)

**Problem.** File listings had no user-controlled sort order.

**Implementation.** Go backend handlers with GORM ordering, parameterized queries with SQL injection protection, query parameter persistence, JavaScript frontend, HTML templates, full test coverage.

**Outcome.** Shipped in v0.10.0. Full-stack: database query to UI state.

---

## What I've Shipped

Cross-functional work spanning four companies — analytics pipelines, AI-integrated tooling, real-time communication, and developer-facing products at 1,200+ DAU.

- Reduced frontend load time from **5s → 3s** and bundle size by **20%** — rearchitected data fetching with RTK Query, eliminated redundant network requests, tuned cache invalidation for a search experience serving **1,200+ DAU**.
- Improved query performance by **25–30%** by designing a shared RTK Query caching layer, normalizing cache keys and coordinating invalidation across features.
- Built Databricks API integration end-to-end — handling auth token rotation, cursor-based pagination across large result sets, and structured error recovery for pipeline failures. Owned from schema design to production deployment.
- Implemented AWS Chime WebRTC communication layer — ICE negotiation, session lifecycle, and reconnection logic under network interruptions. Real-time communication serving concurrent users across unreliable network conditions.
- Shipped a Gemini AI Chrome extension with a `MutationObserver`-based DOM injection strategy resilient to frequent host page updates.

---

## What I Bring

**Backend Ownership**
Observable, failure-aware Go services — error handling, structured logging, and migration safety built in by default.

**Performance Mindset**
I diagnose before optimizing, measure after. Fixed problems include: unbounded memory growth, 5s load times, redundant API calls.

**Product Engineering**
I track what I ship against real usage. DAU, load time, Lighthouse — not closed tickets.

**Remote Collaboration**
IST-based. Async-first, clear PR descriptions, no synchronous check-ins required to stay unblocked.

---

## Engineering Philosophy

**Simplicity is a feature.** The most maintainable system is the one the next engineer can read without asking questions.

**Reliability over cleverness.** Boring, predictable behavior with clear failure modes beats elegant abstractions that collapse under edge cases. The `sync.Map` fix chose a well-understood LRU library over a custom solution for exactly this reason.

**Observability is not optional.** Structured logging and meaningful errors are how you know what's actually happening in production — not just what you think is happening.

**Performance is product.** Latency and load time are product requirements. The 5s → 3s improvement came from treating them as such, not as a post-launch cleanup task.

---

## Stack

~~~
Backend         Go, Node.js, Express
Frontend        React, TypeScript, RTK Query
Data            PostgreSQL, Redis, SQLite, GORM
Infrastructure  AWS, Docker, GitHub Actions
Testing         Vitest, React Testing Library
~~~

---

## How I Work

I own incidents on things I've shipped: postmortem, root cause, fix — not just the symptom.

Async-first. I write decisions down rather than schedule meetings. PRs are small and scoped — reviewers shouldn't need context I didn't provide.

Based in India (IST), working with US and EU teams.

---

## Current Focus

Deepening Go expertise through production work — concurrency patterns, service design, operational reliability. The shift is grounded in real systems, not technology trends.
Contributing to open source when I find something real to fix.

---

## Contact

[LinkedIn](https://linkedin.com/in/krupeshjoshi) · [Email](mailto:krupeshjoshi21@gmail.com)
