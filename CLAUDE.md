# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

@AGENTS.md

## Commands

```bash
npm run dev      # Start development server at localhost:3000
npm run build    # Production build
npm start        # Start production server
npm run lint     # Run ESLint
```

No test framework is configured yet.

## Architecture

**Stack:** Next.js (App Router) + TypeScript + Tailwind CSS v4

The project was scaffolded with `create-next-app` and has not yet been built out. Core expense tracker functionality — components, data models, persistence, and API routes — needs to be implemented.

**Routing:** Uses Next.js App Router (`/app` directory). New routes go in `app/<route>/page.tsx`; API endpoints go in `app/api/<route>/route.ts`.

**Styling:** Tailwind CSS v4 — uses the new `@theme` inline syntax in `globals.css`, not the v3 `tailwind.config.js` approach. Dark mode is handled via CSS custom properties with `prefers-color-scheme`.

**TypeScript:** Strict mode enabled. Path alias `@/*` resolves to the repo root.

**ESLint:** Flat config format (`eslint.config.mjs`), not `.eslintrc`.
