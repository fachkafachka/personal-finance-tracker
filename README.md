# Ledgerly

Ledgerly is a polished, responsive personal finance dashboard built with React, TypeScript, Vite, Recharts, and Lucide icons.

## Features

- Dashboard with balance, income, expenses, savings rate, cash-flow and spending charts.
- Add, edit, delete, search, filter, categorize, and mark recurring transactions.
- Monthly category budgets with visual progress and overspending warnings.
- Cash, Checking, Savings, and Credit Card account balances.
- Week, month, year, and custom-range-ready filtering controls.
- Accessible form labels, validation, empty states, and destructive-action confirmation.
- Seeded sample data so the dashboard is immediately useful.
- Local persistence through `localStorage`, with a clean data layer boundary ready for authentication and cloud sync.

## Run locally

```bash
npm install
npm run dev
```

Then open the local URL printed by Vite. Create a production build with `npm run build`.

## Data and future sync

Transactions and budgets are currently serialized to `localStorage` under `ledgerly-transactions` and `ledgerly-budgets`. The app keeps typed models (`Transaction` and `Budget`) in `src/App.tsx`; these can be moved into a repository/service layer when adding a remote API, authenticated user identity, and sync conflict handling.
