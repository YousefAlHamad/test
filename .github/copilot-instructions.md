# Mona Mayhem Instructions

## Project Overview

- Mona Mayhem is an Astro 6 site for comparing two GitHub contribution graphs in a retro arcade-style battle arena.
- The application lives in `src/`; file-based pages and endpoints live under `src/pages/`.
- The project uses server-side output with the `@astrojs/node` standalone adapter. Preserve this setup when adding API routes or server-only behavior.
- Treat `workshop/` as reference material only. Do not modify it unless a task explicitly requests workshop changes.

## Commands

- Install dependencies: `npm ci`
- Start development server: `npm run dev`
- Build for production: `npm run build`
- Preview a production build: `npm run preview`

## Astro Practices

- Add pages as `.astro` files in `src/pages/`; Astro maps their paths automatically.
- Add API endpoints in `src/pages/api/` and export HTTP method handlers such as `GET`.
- Keep static assets in `public/` and reference them with root-relative paths.
- Prefer Astro components and server-side code by default. Introduce a client framework or hydration directive only when browser-side interactivity requires it.
- Keep server-only secrets in environment variables; never expose them in client-rendered code.
- Run `npm run build` after changes that affect pages, routes, or Astro configuration.