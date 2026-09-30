# momo-guardian-frontend

Consumer demo app for **MoMo Guardian** — the send-money flow with a real-time Safety Check.
Presentation only: **no risk logic lives here**; it calls `momo-guardian-api`.

> Status: scaffold only (no code yet). Proposed stack: React + TypeScript + Vite + Tailwind (see ADR-0002).

## Screens to build
Home · Send money · Safety Check (warn/challenge) · Step-up verification · Result · Activity dashboard · Scam Simulator (demo panel)

## Key docs (in the docs hub)
- User flows: `https://github.com/momo-guardian/momo-guardian-docs/blob/main/01-product/user-flows.md`
- API contract: `https://github.com/momo-guardian/momo-guardian-docs/blob/main/02-architecture/api-contract.md`
- Brand & colors: `https://github.com/momo-guardian/momo-guardian-docs/blob/main/04-brand/brand-guidelines.md`
- Local docs: [`docs/`](docs/)

## Quick start (fill in when initialized)
```bash
cp .env.example .env
npm install
npm run dev
```

## Rules
- Follow the API contract; use `src/mocks/` for offline demo fallback.
- Branches & commits: see org CONTRIBUTING.
