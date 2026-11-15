<p align="center">
  <img src="icon.png" alt="CyberX logo" width="160" />
</p>

# CyberX website

Official marketing website for **[CyberX](https://github.com/Tamilselvan-S-Cyber-Security/Cyber-X)** — a local-first desktop workspace for specialized AI agents.

Developed by **Tamilselvan**. Sponsored by **[Cyber Wolf](https://www.cyberwolf360.in)**.

Live site: [https://mathan0310e.github.io/official/](https://mathan0310e.github.io/official/)

This README is about **using and developing the website only** — not installing the CyberX desktop app.

## Stack

- Vite
- React 19
- TypeScript
- React Router (HashRouter)
- Tailwind CSS 4

## Website usage

### Run locally

```bash
npm install
npm run dev
```

Open the URL Vite prints (usually `http://localhost:5173/`).

### Pages

| Page | Route |
|------|--------|
| Home | `/#/` |
| Agents | `/#/agents` |
| Agent detail | `/#/agents/<id>` (example: `/#/agents/autonomous`) |
| Features | `/#/features` |
| Download | `/#/download` |
| Install guide | `/#/install` |

### Common website tasks

| Task | Where |
|------|--------|
| Edit product copy, agents, download links, FAQs | `src/data.ts` |
| Change page routes / layout shell | `src/App.tsx`, `src/components/SiteLayout.tsx` |
| Edit a page | `src/pages/` |
| Edit UI sections | `src/components/` |
| Edit SVG artwork | `src/illustrations/` |
| Edit styles / tokens | `src/styles/` |
| Replace hero demo video | `public/cyberx-demo.mp4` (see below) |

### Scripts (website)

```bash
npm run dev          # local website server
npm run build        # typecheck + build into dist/
npm run preview      # preview the built website
npm run typecheck    # TypeScript check only
npm run audit        # website layout / interaction / contrast checks
```

## Hero demo video

The home hero plays the CyberX desktop demo recording.

| Asset | Path in this repo |
|-------|-------------------|
| Video (source) | `public/cyberx-demo.mp4` |
| Poster image | `public/cyberx-demo-poster.jpg` |
| Used in | `src/components/HeroVideo.tsx` |
| Served URL in the site | `./cyberx-demo.mp4` |

Vite copies everything under `public/` to the build root, so after `npm run build` the video is also available as `dist/cyberx-demo.mp4`.

### Replace the video

1. Put the new file at **`public/cyberx-demo.mp4`** (same name, or update `HeroVideo.tsx` if you rename it).
2. Optionally update **`public/cyberx-demo-poster.jpg`** to match the first frame.
3. Refresh `npm run dev` — no import change is required when the filename stays the same.

Playback notes (website behaviour):

- Muted autoplay + loop (required by browsers without a user gesture)
- Mounts when the hero is near the viewport
- Pauses when the tab is hidden or `prefers-reduced-motion: reduce` is set

## Project structure

```
public/
  cyberx-demo.mp4           Hero demo video (root of public assets)
  cyberx-demo-poster.jpg    Video poster frame
  icons/                    Favicon and app icons
  manifest.webmanifest      PWA metadata
src/
  App.tsx                   Routes
  data.ts                   Website content + download metadata
  pages/                    One file per website page
  components/               Layout and sections
  illustrations/            SVG artwork
  hooks/                    Shared React hooks
  styles/                   Tokens, globals, animations, responsive
scripts/                    Website audit helpers
```

## Content source of truth

All product facts shown on the site (versions, agent text, release URLs, checksums) live in **`src/data.ts`**. Update that file when the website copy or download links change.

## Related repositories

- Desktop app + installers: [Tamilselvan-S-Cyber-Security/Cyber-X](https://github.com/Tamilselvan-S-Cyber-Security/Cyber-X)
- This repo: website only
