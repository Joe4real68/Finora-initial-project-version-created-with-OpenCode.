# Finora — Know your money. Manage it wisely.

> Finora is a smart personal finance tracker that helps you understand your income, control your spending, and manage your money intentionally.

**Christian-focused:** Finora helps you manage your money wisely while giving you an optional, simple way to track your tithe and practise faithful financial stewardship.

## 1. Product Overview

Finora is a personal income and expense management app for individuals, freelancers, service providers, small business owners, and anyone who wants better control over their finances.

It lets users record income and expenses, monitor financial activity, identify spending patterns, and receive useful insights about their financial behaviour.

Core differentiator: **intelligent spending insights** with an **optional automatic tithe-tracking feature** for Christians. When enabled, the app automatically calculates 10% of recorded income and accumulates it until marked as paid.

Goal: not just record transactions, but help users become **more aware, disciplined, and intentional with money.**

Full spec: see `Docs/Finora.md`.

## 2. Problem It Solves

Many people — especially those with irregular income — struggle to track how much they earn, spend, and have left. Spending happens gradually without a clear picture, leading to overspending discovered too late.

Finora provides a simple, intelligent way to track income/expenses, monitor patterns, and get insights that encourage better decisions. For Christians, it removes the stress of manually calculating tithe from different income sources.

## 3. Target Users

- Freelancers and service providers (variable income, multiple clients)
- Small business owners (regular customer income)
- Employees (salary, personal spending control)
- Students and young adults (learning financial habits)
- Christian users (tithe calculation, accumulation, monitoring)

## 4. Key Features

### User Account
Create account, log in/out, manage profile, set preferred currency, private access to financial data.

### Dashboard
Financial home screen — at-a-glance overview:
- Available Balance (income − expenses)
- Total Income (selected period)
- Total Expenses (selected period)
- Tithe Balance (only if enabled)
- Financial Insight (short observation, e.g. “You've earned ₦500,000 this month and spent ₦180,000. Your spending is currently within your usual range.”)

### Income Tracking
Record: amount, source, category, date, optional note.
E.g. Client Payment, Salary, Freelance Project, Business Sales. Auto-updates totals and balance.

### Expense Tracking
Record: amount, category, date, optional note.
Default categories: Food, Transportation, Bills, Rent, Shopping, Entertainment, Business, Education, Health, Giving, Other + custom categories.

### Transaction History
Complete history with type, amount, category/source, date, note. Search, filter by type/category/date range, edit, delete.

### Spending Insights (key feature)
Pattern analysis — inform and encourage, not shame:
- High spending, unusual spending, trends, income-vs-spending ratio, positive behaviour
- E.g. “You've spent 72% of your recorded income this month.”

### Financial Alerts
Helpful, not excessive, user-controllable:
spending alerts, insights, income updates.

### Tithe Tracker (optional)
Turn on/off. Auto-calculates 10% of recorded income and accumulates.
E.g. ₦100,000 income → ₦10,000 tithe; + ₦50,000 income → ₦15,000 total.
Does not interfere with core experience when off.

### Tithe Payment & History
Mark accumulated tithe as paid → records payment + date, resets current balance, keeps history.

### Tithe Reset Preferences
Weekly / Monthly / Manual. Manual = accumulate until paid. Never auto-erase unpaid tithe on period change.

### Periods, Summaries, Reports
Periods: Today, This week, This month, Last month, This year, Custom range.
Summary per period: total income/expenses/balance, spending by category, income by source, tithe accumulated, major patterns.
Reports: monthly income/expenses, by category, sources, tithe history, balance trends.

### Categories
Defaults + add/rename/remove custom categories.

### Future (Phase 2)
AI Financial Assistant (query your own data), Affordability / Spending Check (“Can I afford ₦100,000 phone?”), Savings Goals, advanced insights, detailed reports, custom notifications, recurring income/expenses.

## 5. MVP Scope (v0.1)

Essential for first version:
1. Account creation and login
2. Dashboard
3. Add income
4. Add expenses
5. Transaction history
6. Income and expense summaries
7. Spending categories
8. Basic spending insights
9. Tithe Tracker
10. Mark tithe as paid
11. Tithe history
12. Basic financial settings

Deferred to Phase 2: AI assistant, affordability checker, savings goals, advanced insights, detailed reports, custom notification settings, recurring transactions.

## 6. Typical User Journey

Sign up → Set up profile → Add income → Add expenses → View balance → Review spending → Receive insight → Track tithe if enabled → Mark tithe as paid → Continue tracking

Recording a transaction should take only seconds.

## 7. UX Principles

- **Simple:** no financial knowledge required
- **Clean:** no clutter
- **Private:** secure and personal
- **Helpful:** insights explain behaviour
- **Non-judgmental:** encourage, not guilt
- **Faith-friendly:** Christian features natural and optional

## 8. Project Structure

```
Finora/
  Docs/
    Finora.md   # Product Requirements Document (source of truth)
  README.md     # This file
```

No application code yet — v0.0.1 is docs + README baseline.

## 9. How to Run

This is currently a **docs-only baseline (v0.0.1)** — there is no app code to build yet.

To view the project:

```bash
git clone https://github.com/<your-username>/Finora.git
cd Finora
# Read the overview
# - README.md (this file)
# - Docs/Finora.md (full PRD)
```

Once implementation starts, run instructions will be added here (e.g. `npm install`, `npm run dev`).

Suggested next steps:
1. Choose stack (e.g. web / mobile / API + DB)
2. Define data model: User, Transaction, Category, TitheSetting, TithePayment
3. Implement MVP items 1–12 above
4. Add tests for balance, tithe 10%, period filtering

## 10. Success Criteria

A user can quickly record income/expenses, see available balance, see where money goes, recognise patterns, receive useful insights, track tithe if enabled, review history, and feel more informed and intentional.

## 11. Vision

Grow from tracker → companion: **Track → Understand → Plan → Decide → Improve**

Long-term: help people develop a clearer relationship with money, whether salaried, freelance, business, student, or using stewardship features.

---
*Version: v0.0.1 — initial docs baseline. Source: `Docs/Finora.md`.*
