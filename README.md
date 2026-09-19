# ExecutiveFlow

Your AI Executive Assistant for a Busy Business Life.

ExecutiveFlow is a modern, AI-powered productivity platform for busy business owners, executives and managers. It brings your emails, meeting notes, tasks and schedule into one clean, professional workspace — inspired by the aesthetics of Notion, Linear and Slack.

![ExecutiveFlow dashboard](src/assets/hero-dashboard.jpg)

## What it does

- **Smart Email Generator** — describe the purpose, pick a recipient type and tone (Professional, Friendly, Persuasive or Formal), and get an instant, polished draft you can copy, regenerate or save as a template.
- **Meeting Notes Summarizer** — paste notes or transcripts and get an executive summary, key points, decisions, action items with owners, and follow-up recommendations. Export to PDF or share with your team.
- **Smart Task Planner & Scheduler** — create tasks manually or with AI, prioritise High/Medium/Low, view daily/weekly/monthly schedules, and let AI suggest what to focus on next.
- **Calendar** — week view with conflict detection and one-click scheduling fixes.
- **Analytics** — productivity score, time breakdown and hours-saved trends.

## Built with

- [TanStack Start](https://tanstack.com/start) — full-stack React 19 framework
- TypeScript
- Tailwind CSS v4 with an oklch design-token system (deep navy / white / soft gray / electric blue)
- shadcn/ui components
- Recharts for analytics
- Sonner for toasts

## Getting started

```sh
npm i
npm run dev
```

Open the app at the local dev URL. The landing page introduces the product; the dashboard (via **Get started** / **Start Free Trial**) contains the full workspace experience with realistic sample data.

## Project structure

```
src/
├── assets/            # Hero image and static assets
├── components/
│   ├── dashboard/     # DashboardShell (sidebar, header, nav)
│   └── ui/            # shadcn/ui primitives
├── lib/
│   ├── demo-data.ts   # Types and realistic sample data
│   └── ai-mock.ts     # Simulated AI generation (email, summaries, tasks)
├── routes/            # File-based routes (landing + 7 dashboard pages)
└── styles.css         # Design tokens, themes and utilities
```

## Notes

- This build is a **polished demo**: AI responses are simulated with realistic delays and all data is sample data — no backend, auth or persistence is wired up yet.
- Light theme is the default; a dark theme toggle is included.
- PDF export, sharing and billing actions surface "available on the full version" toasts.

## Roadmap ideas

- Wire the email generator, summarizer and task suggestions to a real LLM
- Accounts, secure auth and per-user workspaces
- Calendar and email integrations
- Team collaboration and shared workspaces

---

Built with [Lovable](https://lovable.dev).
