# Folder Structure

```
momo-guardian-frontend/
├── docs/                      # Frontend-specific docs (component inventory, state map, decisions)
├── public/                    # Static files served as-is
│   ├── fonts/
│   └── images/                # favicon, social preview
├── src/
│   ├── app/                   # App shell: routing, providers, entry
│   ├── components/            # Reusable, feature-agnostic UI
│   │   ├── ui/                # Buttons, inputs, cards, modal, badge
│   │   ├── layout/            # Header, bottom nav, page container
│   │   ├── transaction/       # Amount input, recipient field, receipt
│   │   ├── risk/              # Risk meter, reason list, level badge
│   │   └── verification/      # Countdown, re-confirm input, approval card
│   ├── features/              # Feature modules (own components + hooks + logic)
│   │   ├── send-money/
│   │   ├── safety-check/
│   │   ├── step-up-verification/
│   │   ├── risk-explainer/
│   │   ├── activity-dashboard/
│   │   └── scam-simulator/    # Demo control panel
│   ├── hooks/                 # Shared hooks
│   ├── lib/                   # Utilities (formatting GHS, phone validation)
│   ├── services/              # API client (typed to the contract)
│   ├── store/                 # Global state
│   ├── types/                 # Shared TS types (mirror API contract)
│   ├── config/                # Env, feature flags, risk-level → UI mapping
│   ├── mocks/                 # Offline fallback responses for demo safety
│   ├── styles/                # Global CSS, design tokens (from brand doc)
│   └── assets/{icons,illustrations}
├── tests/{unit,e2e}/
└── .github/workflows/         # CI: lint, typecheck, test
```
Planned root files (create at init): `package.json`, `vite.config.ts`, `tsconfig.json`, `.env.example`, `.gitignore`, `.eslintrc`, `.prettierrc`.
