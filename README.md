# Wooseong Ham

**Dev team lead & product builder** — I take products from an empty repository to something people pay for, and then keep them running.

Most of what I build lives in private repositories, so this page is the map.

---

## What I do

**Own products end to end.** Product decisions, database schema, API, frontend, the native shell, deployment, and the on-call that follows. When something breaks at 11pm, I'm the one who fixes it.

**Lead a small dev team.** Code review, release process, and keeping a codebase that more than one person can work in — which mostly means boring, readable code and migrations that actually finish.

**Build for people who aren't developers.** Small business owners, gym members, brand marketers. The bar is "my mother can use this", not "the demo worked".

---

## Tech

**Frontend** &nbsp;·&nbsp; Next.js (App Router) &nbsp;·&nbsp; React 19 &nbsp;·&nbsp; SvelteKit &nbsp;·&nbsp; TypeScript &nbsp;·&nbsp; Tailwind CSS

**Backend** &nbsp;·&nbsp; Node.js &nbsp;·&nbsp; Prisma &nbsp;·&nbsp; PostgreSQL &nbsp;·&nbsp; Supabase &nbsp;·&nbsp; REST APIs

**Mobile** &nbsp;·&nbsp; Android (Kotlin) &nbsp;·&nbsp; watchOS (Swift) &nbsp;·&nbsp; FCM push &nbsp;·&nbsp; deep linking

**Testing** &nbsp;·&nbsp; Vitest &nbsp;·&nbsp; Playwright &nbsp;·&nbsp; Zod

**Infra** &nbsp;·&nbsp; Vercel &nbsp;·&nbsp; GitHub Actions

A large share of my recent work is migration — Next.js 13 → 16, React 18 → 19, Tailwind 3 → 4, Prisma 7 — across four codebases at once. Keeping a shipping product on a moving framework is its own skill.

---

## Selected work

Products I own end to end and still maintain in production. The code is private, so I describe scope rather than link repositories.

### 기준 (GI-JUN) — all-in-one HR SaaS for small teams
**[gijun.co.kr](https://www.gijun.co.kr)** · ~96,000 lines of TypeScript across 900+ files

A multi-tenant SaaS covering attendance, leave, expense approval, e-contracts, and onboarding — the HR work a small company has no dedicated team for.

- **Korean labor law encoded as product.** Statutory leave accrual, 12 legally mandated leave types with annual caps, and a daily cron that warns admins before compliance deadlines pass. Getting this wrong costs a customer real money, so the rules live in tested code rather than in a spreadsheet.
- **Multi-tenant security.** Row-level isolation in Postgres, encrypted PII, TOTP two-factor enforced at the database layer, and writes restricted to server-side APIs.
- **Four platforms, one codebase.** Next.js 16 / React 19 web app, an Electron desktop client, and Android and iOS shells, each with its own CI pipeline.
- **AI where it removes work, not where it demos well.** Payroll preparation that checks rules and diffs against last month before a human approves, first-line answers for support inquiries with escalation when unresolved, and weekly report drafts.
- **Growth built in.** A content site with 35+ articles, 16 downloadable HR document templates, and 15 free calculators (severance, overtime, insurance) that bring in the small businesses the product is for.

### 리뷰노트 — review campaign platform
Connects brands with reviewers. Next.js service with Prisma, a separate API layer on Supabase, an admin console for campaign review and settlement, and a native Android client. The codebase spans web, API, admin, and mobile as four coordinated repositories.

### 라곰트레이닝 — training log and community app
Built and maintained solo across roughly 2,000 commits. SvelteKit + Supabase, with an Android shell and a watchOS companion that tracks workouts on the wrist. Used daily by a real gym — which is the fastest feedback loop I've worked in.

---

## Writing

I write about what I run into while building, at [velog.io/@wsham](https://velog.io/@wsham).

---

## Contact

**Email** &nbsp;[wooseongham@gmail.com](mailto:wooseongham@gmail.com) &nbsp;&nbsp;·&nbsp;&nbsp; **Location** &nbsp;Seoul, South Korea
