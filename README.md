# janae-site

Personal website built with Astro. Dark mode, soft pink accent, typography-forward.

## Setup

```bash
# Install dependencies
npm install

# Start the dev server (http://localhost:4321)
npm run dev

# Build for production
npm run build

# Preview the production build locally
npm run preview
```

## Project structure

```
janae-site/
├── public/             # Static assets (favicon, etc.)
├── src/
│   ├── components/     # Reusable Astro components
│   │   ├── Nav.astro
│   │   ├── Waveform.astro
│   │   └── Section.astro
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   └── index.astro       # Main page — 4 sections: Intro, Work, Free Time, Now Playing
│   └── styles/
│       └── global.css        # Design tokens + base styles
├── astro.config.mjs
├── package.json
└── README.md
```

## Customizing

All design tokens live in `src/styles/global.css` at the top under `:root`.
Change one CSS variable and the whole site updates.

```css
--accent: #f9a8d4;          /* swap this to change the accent color */
--bg: #0a0a0a;              /* background */
--text-primary: #fafafa;    /* primary text */
```

## Deploying

The fastest path: push to GitHub, then connect the repo at vercel.com.
Vercel auto-detects Astro, builds, and deploys. Every `git push` redeploys.
