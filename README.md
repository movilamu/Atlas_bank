# Atlas — Digital Banking UI

A polished, responsive digital banking prototype built with React, TypeScript, Vite, Recharts and Lucide icons. Designed as a presentation-ready frontend with realistic account, payment, card, transaction, savings, insight and document workflows.

## Important: demo-only financial flows

This repository is a **frontend prototype**, not a real banking system. Account balances and activity are sample data. Transfers and top-ups only update in-memory UI state and do not move money. Authentication, authorization, persistent database storage, real payment rails, KYC/AML, fraud controls, audit trails, secrets management and regulatory controls are not implemented. Do not enter real personal or financial information and do not use this prototype to handle real funds.

## Run locally

Requires Node.js 20 or newer.

```bash
npm install
npm run dev
```

Open the local URL shown by Vite.

## Production build

```bash
npm run build
npm run preview
```

## Deploy to Vercel from GitHub

1. Create a new GitHub repository, for example `atlas-banking-ui`.
2. Extract this project and push the files to the repository root.
3. In Vercel, choose **Add New → Project**, import the GitHub repository and use these settings:
   - Framework preset: **Vite**
   - Build command: `npm run build`
   - Output directory: `dist`
   - Install command: `npm install`
4. Click **Deploy**. The included `vercel.json` supports client-side navigation fallback.

No environment variables are required for the demo UI.

## Tech stack

- React + TypeScript
- Vite
- Recharts
- Lucide React
- Custom responsive CSS

## Before any real-world banking deployment

Use a proper backend and database, server-side authorization and input validation, audited transfer workflows with idempotency and double-entry ledger accounting, an established identity/authentication provider, secure session handling, secrets stored only in server environment variables, monitoring, automated tests, and security/compliance review. Never trust a client-side balance or transaction record.
