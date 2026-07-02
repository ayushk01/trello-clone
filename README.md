# trello-clone

A Trello-style kanban app — organizations, boards, lists, and cards with drag-and-drop
reordering, an activity/audit log, board covers from Unsplash, and Stripe-powered board
limits. Built end-to-end as a hands-on deep dive into the Next.js 14 App Router and
server actions.

**Live demo:** https://trelllo-silk.vercel.app

## Stack

- **Next.js 14** (App Router, server actions) · React 18 · TypeScript
- **Prisma + MySQL** — boards, lists, cards, audit log
- **Clerk** — authentication & organizations
- **@hello-pangea/dnd** — drag-and-drop for lists and cards
- **Stripe** — subscription unlock for unlimited boards
- Tailwind CSS · Radix UI · Zustand · TanStack Query · Zod

## Run locally

```bash
npm install
cp .env.example .env.local   # Clerk, database, Unsplash, Stripe keys
npx prisma generate && npx prisma db push
npm run dev
```

> Yes — the demo URL has three L's (`trelllo`). The typo shipped first and stuck.
