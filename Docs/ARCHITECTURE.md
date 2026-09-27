# Finora — Implementation Architecture (Phased Folders)

Source of truth: `Docs/Finora.md` (PRD §§1–28). Stack-agnostic `src/` layout — works for monolith or API+UI split.

Core domain: `User → Transaction{income|expense} → Category, TitheSetting → TithePayment`

## Phase 0 — Baseline (done, v0.0.1)
- `README.md`, `Docs/Finora.md`, `.github/workflows/ci.yml`
- No app code.

## Phase 1 — Foundation: Account + Settings (PRD §5.1)
- `src/auth/` — signup, login, logout, session, private per-user scoping
- `src/users/` — profile, preferred currency
- `src/settings/` — tithe on/off, reset pref weekly/monthly/manual, notification prefs stub
- `src/db/` — User, UserSettings tables, migrations, seeds
- `src/ui/auth/`, `src/ui/settings/` — login, signup, profile, settings screens
- `tests/auth/`, `tests/users/`, `tests/settings/`
- Done when: private login works, currency set, tithe toggle persists.

## Phase 2 — Core Money (PRD §7, §8, §9, §15, §17)
- `src/categories/` — defaults: Food, Transportation, Bills, Rent, Shopping, Entertainment, Business, Education, Health, Giving, Other + custom add/rename/remove
- `src/transactions/` — income{amount,source,category,date,note}, expense{amount,category,date,note}, CRUD, search, filter by type/category/date-range, edit/delete, periods: today/week/month/last-month/year/custom
- `src/summaries/` — totalIncome, totalExpenses, balance (= income−expenses) per period, by-category, by-source
- `src/ui/transactions/`, `src/ui/categories/` — sub-5-second add, history list
- `tests/categories/`, `tests/transactions/`, `tests/summaries/`
- Done when: add in seconds, balance correct, history filters work.

## Phase 3 — Understand (PRD §6, §10, §11, §16)
- `src/dashboard/` — balance, income, expenses, titheBalance (if enabled), 1-line insight
- `src/insights/` — rules: high/unusual/trend/income-vs-%/positive, non-judgmental copy (e.g. “spent 72% of income”)
- `src/alerts/` — 80%-spent, food-above-average, income-up; user-controllable, not excessive
- `src/reports/` — monthly income/expense, trends stub
- `src/ui/dashboard/`, `src/ui/insights/`
- `tests/dashboard/`, `tests/insights/`
- Done when: at-a-glance dashboard + helpful insight, e.g. “₦500k earned, ₦180k spent, within usual range”.

## Phase 4 — Tithe Tracker (PRD §12, §13, §14)
- `src/tithe/` — auto 10% on income create, accumulate, markPaid{date,reset,keep-history}, never auto-erase unpaid on period rollover, history list
- `src/ui/tithe/` — balance card, mark-paid button, history
- `tests/tithe/` — 100k→10k, +50k→15k, paid-reset, rollover keeps unpaid
- Done when: off = invisible, on = correct accumulation.

## Phase 5 — Placeholders (PRD §18–22, no impl yet)
- `src/ai-assistant/` — query own data only (not generic advice)
- `src/affordability/` — can-I-afford check (balance, recent income/expenses, patterns)
- `src/savings-goals/` — goal, current/target, %
- `src/recurring/` — recurring income/expenses stub
- `src/notifications/` — record income/expense reminders, tithe accumulated, summary ready

## Folder tree (scaffolded with .gitkeep)
```
Finora/
  Docs/Finora.md
  Docs/ARCHITECTURE.md
  README.md
  .github/workflows/ci.yml
  src/auth users settings categories transactions summaries dashboard insights alerts reports tithe db/
  src/ai-assistant affordability savings-goals recurring notifications/
  src/ui/auth settings transactions categories dashboard insights tithe/
  tests/auth users settings categories transactions summaries dashboard insights tithe/
```
