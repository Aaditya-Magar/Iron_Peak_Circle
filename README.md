# Iron Peak Circle

A portfolio website built to showcase a premium gym marketing experience with a modern frontend stack.

This repository contains a fully static frontend built with React, TypeScript, Tailwind CSS, TanStack Router, and Framer Motion. It is designed as a portfolio piece to demonstrate how I build polished, production-ready web interfaces and route-driven user experiences.

## What this project includes

- **Portfolio-ready landing pages** for home, classes, trainers, schedule, membership, about, gallery, and contact.
- **Responsive, mobile-first UI** with dark, premium styling and red accent calls-to-action.
- **Static content driven by `src/lib/data.ts`** so the site is fully client-rendered with no backend required.
- **Reusable UI components** in `src/components/` and `src/components/ui/`.
- **Page transitions, scroll effects, and motion design** with Framer Motion.
- **Vercel-ready deployment** via the included `vercel.json` rewrite rule.
- **Custom favicon** added in `public/favicon.svg`.

## How I built it

- Used **TanStack Router** file-based routing to keep pages and metadata organized under `src/routes/`.
- Kept site content reusable by storing trainers, classes, membership plans, and testimonials in `src/lib/data.ts`.
- Built components with **Tailwind CSS** and custom utility styles in `src/styles.css`.
- Added a polished **404 experience** and consistent brand styling across every page.
- Configured the app to behave as a static SPA with a `vercel.json` rewrite so deep routes work on Vercel.
- Added a browser-friendly SVG favicon that matches the site's dark gym aesthetic.

## Tech stack

- React 19
- TypeScript
- Vite 7
- Tailwind CSS 4
- TanStack Router
- Framer Motion
- Lucide Icons

## Local development

```bash
npm install
npm run dev
```

Open `http://localhost:5173` after the dev server starts.

## Build and preview

```bash
npm run build
npm run preview
```

## Vercel deployment

This project is ready for Vercel deployment.

1. Push the repo to GitHub.
2. Import the project at https://vercel.com/new.
3. Set the build command to:

```bash
npm run build
```

4. Set the output directory to:

```text
dist
```

Vercel will detect the Vite app automatically. The included `vercel.json` rewrites all routes to `index.html` so the static SPA works on refresh and deep links.

## Project structure

```text
src/
├── components/          # Reusable UI and layout components
├── lib/                 # Static site data for pages and sections
├── routes/              # File-based routes and page metadata
└── styles.css           # Tailwind CSS configuration and custom utilities
public/
└── favicon.svg          # Browser favicon asset
```

## Notes

- This is a **portfolio project** and not a real gym brand.
- All content is fictional and built for design demonstration.
- The app is fully static and does not require any backend services.

## Favicon

A custom gym-themed SVG favicon is included in `public/favicon.svg` and linked in `src/routes/__root.tsx`.

## Ready for production

The app is configured for static deployment, optimized for Vercel, and powered by modern web tooling.
