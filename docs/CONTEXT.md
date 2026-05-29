# Budget Tracker - Context Document

## 1) Project Overview
- **Project Name:** Budget Tracker
- **Product Type:** Mobile-first web application
- **Primary Goal:** Help users track daily income/expense against a daily budget in real time.
- **Target Outcome:** Users can quickly see whether they are within budget, near limit, or over budget.

## 2) Problem Statement
Users need a simple way to:
- Set today's budget
- Log daily income/expense quickly
- See remaining budget status clearly

This project also uses a **public feedback loop** (TikTok comments) to prioritize upcoming features.

## 3) MVP Scope (v1)
1. Daily budget setup
2. Quick transaction logging (income/expense, amount, category, note, timestamp)
3. Daily summary (income total, expense total, net remaining)
4. Daily transaction list (view/edit/delete)
5. Basic category insight for the day

## 4) Out of Scope (for MVP)
- Multi-user collaboration
- Advanced financial analytics/report exports
- Complex recurring transaction engine
- Full gamification system

## 5) Recommended Industry-Standard Stack
- **Frontend:** Next.js (App Router), TypeScript, Tailwind CSS
- **UI System:** shadcn/ui
- **Forms/Validation:** React Hook Form + Zod
- **Backend/API:** Next.js Route Handlers
- **Database:** PostgreSQL + Prisma
- **Hosting:** Vercel
- **Monitoring:** Sentry
- **Analytics:** PostHog

## 6) Delivery Principles
- Mobile-first UX
- Fast data entry (few taps)
- Clear status language and color states
- Incremental delivery with short feedback cycles
- Track every feature request in a structured backlog

## 7) Task Tracker (Execution Board)
| ID | Task | Status | Owner | Notes |
|---|---|---|---|---|
| T1 | Finalize MVP scope and acceptance criteria | ✅ Done | Founder + AI | Captured in README and this context doc |
| T2 | Define screen flow (Home, Add, History) | ⏳ Next | Founder | Create mobile wireframes in Google Stitch |
| T3 | Scaffold project (Next.js + TypeScript + Tailwind) | ⏳ Next | AI | Initialize repo structure |
| T4 | Set up DB schema (daily_budgets, transactions) | ⏸ Planned | AI | Use Prisma migrations |
| T5 | Implement MVP core features | ⏸ Planned | AI | Build in small milestones |
| T6 | Instrument analytics + feedback loop process | ⏸ Planned | Founder + AI | Connect comment ideas to backlog |

## 8) Immediate Next Step
1. Design the mobile-first user flow in Google Stitch (Home, Add Transaction, History).
2. Lock the MVP acceptance criteria for each screen.
3. Start implementation by scaffolding the Next.js project and base folder structure.

## 9) Definition of Done (MVP)
- User can set daily budget and log transactions on mobile.
- App shows real-time daily remaining/over-budget status.
- Core flow is usable without onboarding instructions.
