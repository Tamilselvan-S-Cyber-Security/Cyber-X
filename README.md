# CyberX Website

Official product website for **CyberX** — a local-first desktop AI agent workspace.

| Detail | Value |
|--------|--------|
| **Live website** | [https://cyberx.cyberwolf360.in/](https://cyberx.cyberwolf360.in/) |
| **Desktop app repo** | [Tamilselvan-S-Cyber-Security/Cyber-X](https://github.com/Tamilselvan-S-Cyber-Security/Cyber-X) |
| **Release page** | [CyberX releases](https://github.com/Tamilselvan-S-Cyber-Security/Cyber-X/releases/tag/CyberX) |
| **Developer** | Tamilselvan |
| **Sponsor** | [Cyber Wolf](https://www.cyberwolf360.in) |
| **Sponsor site** | [https://www.cyberwolf360.in](https://www.cyberwolf360.in) |

This repository is the **website only** (pages, UI, demo video, download links). Use it to view or edit what the live site shows.

---

## Website pages

| Page | Live URL | Route | Contents |
|------|----------|--------|----------|
| **Home** | [cyberx.cyberwolf360.in/#/](https://cyberx.cyberwolf360.in/#/) | `/#/` | Hero, demo video, trust strip, desktop tour, highlighted agents, final CTA |
| **Agents** | [cyberx.cyberwolf360.in/#/agents](https://cyberx.cyberwolf360.in/#/agents) | `/#/agents` | All agent roles (highlighted + classic) with links to detail pages |
| **Agent detail** | […/#/agents/autonomous](https://cyberx.cyberwolf360.in/#/agents/autonomous) | `/#/agents/<id>` | Role summary, focus list, related agents, download CTA |
| **Features** | [cyberx.cyberwolf360.in/#/features](https://cyberx.cyberwolf360.in/#/features) | `/#/features` | Capabilities + four-stage “How it works” path |
| **Download** | [cyberx.cyberwolf360.in/#/download](https://cyberx.cyberwolf360.in/#/download) | `/#/download` | OS auto-detect, Windows/Linux builds, SHA-256 verify |
| **Install** | [cyberx.cyberwolf360.in/#/install](https://cyberx.cyberwolf360.in/#/install) | `/#/install` | Setup guide section + FAQ |

---

## Home page contents

| Section | Details |
|---------|---------|
| **Hero** | Brand intro, CTAs to Download / Agents, OS-aware meta (platform · version · size) |
| **Demo video** | Desktop workspace recording from `public/cyberx-demo.mp4` |
| **Trust strip** | Platform, Windows/Linux versions, agents, local storage, free |
| **Desktop tour** | Interactive mock: Projects → Agents → AI model → Task |
| **Highlighted agents** | Autonomous, Security, Development cards |
| **Final CTA** | Download build / browse agents |

---

## Agents

| Agent | Status | Route | Summary | Focus |
|-------|--------|--------|---------|--------|
| **Autonomous** | Highlighted | `/#/agents/autonomous` | Run queued tasks with less hand-holding | Auto mode, local folder, multi-step handoff |
| **Security** | Highlighted | `/#/agents/security` | Security specialist for reviews and hardening | Reviews, hardening, risk-oriented tasks |
| **Development** | Highlighted | `/#/agents/development` | Build and change code in the project | Implement, refactor, local project work |
| **Red Team** | Classic | `/#/agents/red-team` | Offensive security perspective | Attack-path style tasks, adversary reviews |
| **Blue Team** | Classic | `/#/agents/blue-team` | Defensive / protection workflows | Protection tasks, detection-minded analysis |
| **White Hat** | Classic | `/#/agents/white-hat` | Ethical security work | Ethical assessments, responsible-style tasks |
| **SOC Analyst** | Classic | `/#/agents/soc` | Organize and investigate security tasks | Investigate, organize findings, triage |

Live examples:

- [Autonomous](https://cyberx.cyberwolf360.in/#/agents/autonomous)
- [Security](https://cyberx.cyberwolf360.in/#/agents/security)
- [Development](https://cyberx.cyberwolf360.in/#/agents/development)

---

## Features page contents

### Capabilities

| # | Title | Details |
|---|--------|---------|
| 01 | Local project workspace | Open / create project folders; remove recent folders without deleting files |
| 02 | Configurable AI agents | Add an agent; select its AI; open the agent workspace |
| 03 | Voice and text interaction | Text prompts; voice input adds spoken words to the message box |
| 04 | Prompt queue control | Edit / delete pending prompts; Auto mode sends when the agent is free |

### How it works

| Stage | Label | Lead |
|-------|--------|------|
| 01 | Open your project | Start from the folder you already work in |
| 02 | Add your agent | Give the workspace a role to work from |
| 03 | Choose your AI | Decide which model answers for that agent |
| 04 | Assign your task | Hand over the work by typing or speaking |

---

## Download page contents

| Platform | Version | Format | Size | File | SHA-256 |
|----------|---------|--------|------|------|---------|
| Windows x64 | 0.1.1 | Setup EXE | 129 MB | `CyberX-0.1.1-win-x64-setup.exe` | `ae1c079248f54319755577a18e9df1228d20ab38f97a0f008e94b1fc3142b8a0` |
| Linux x64 | 0.1.0 | tar.gz archive | 161 MB | `CyberX-0.1.0-linux-x64.tar.gz` | `de14f01d26e32f42e40bf443c907e069f13a824cbe50b1e349939e51f70c09bb` |

| Download feature | Details |
|------------------|---------|
| Live page | [https://cyberx.cyberwolf360.in/#/download](https://cyberx.cyberwolf360.in/#/download) |
| OS auto-detect | Pre-selects Windows or Linux; visitor can switch |
| Windows installer URL | [GitHub release asset](https://github.com/Tamilselvan-S-Cyber-Security/Cyber-X/releases/download/CyberX/CyberX-0.1.1-win-x64-setup.exe) |
| Linux archive URL | [GitHub release asset](https://github.com/Tamilselvan-S-Cyber-Security/Cyber-X/releases/download/CyberX/CyberX-0.1.0-linux-x64.tar.gz) |
| Verify (Windows) | `Get-FileHash ".\CyberX-0.1.1-win-x64-setup.exe" -Algorithm SHA256` |
| Verify (Linux) | `sha256sum CyberX-0.1.0-linux-x64.tar.gz` |
| Hosted on | GitHub Releases · no login required |

Source of truth for these values: `src/data.ts` (`DOWNLOADS`).

---

## Hero demo video

| Item | Path / value |
|------|----------------|
| Video (repo) | [`public/cyberx-demo.mp4`](public/cyberx-demo.mp4) |
| Poster (repo) | [`public/cyberx-demo-poster.jpg`](public/cyberx-demo-poster.jpg) |
| Component | [`src/components/HeroVideo.tsx`](src/components/HeroVideo.tsx) |
| Browser URL | `./cyberx-demo.mp4` |
| After build | `dist/cyberx-demo.mp4` |
| Shown on | Home hero — [https://cyberx.cyberwolf360.in/#/](https://cyberx.cyberwolf360.in/#/) |

**Replace the video:** overwrite `public/cyberx-demo.mp4` (and optionally the poster), then refresh `npm run dev`.

Playback: muted autoplay + loop; mounts near viewport; pauses when the tab is hidden or `prefers-reduced-motion` is on.

---

## Tech stack

| Tool | Role |
|------|------|
| Vite | Build / dev server |
| React 19 | UI |
| TypeScript | Types |
| React Router (HashRouter) | Multi-page routes |
| Tailwind CSS 4 | Styling |

---

## Run the website locally

```bash
npm install
npm run dev
```

Open the URL Vite prints (usually `http://localhost:5173/`).

| Script | Purpose |
|--------|---------|
| `npm run dev` | Local development server |
| `npm run build` | Typecheck + production build → `dist/` |
| `npm run preview` | Preview the built site |
| `npm run typecheck` | TypeScript only |
| `npm run audit` | Layout + interaction + contrast checks |

---

## Project structure

```
public/
  cyberx-demo.mp4              Hero demo video
  cyberx-demo-poster.jpg       Video poster
  icons/                       Favicons and app icons
  og-image.png                 Open Graph image
  manifest.webmanifest         PWA metadata
  robots.txt
  sitemap.xml
src/
  App.tsx                      Hash routes for all pages
  data.ts                      Website copy + download metadata
  pages/                       Home, Agents, Features, Download, Install, 404
  components/                  Nav, hero, sections, download UI, layout
  illustrations/               SVG artwork and agent emblems
  hooks/                       Reveal, OS download detect, etc.
  styles/                      Tokens, globals, animations, responsive
scripts/                       Website audit helpers
```

---

## Edit website content

| Change | File / folder |
|--------|----------------|
| Agents, features, FAQs, download URLs, versions, checksums | `src/data.ts` |
| Routes | `src/App.tsx` |
| Page layouts | `src/pages/` |
| Sections / UI | `src/components/` |
| SVG art | `src/illustrations/` |
| Design tokens / CSS | `src/styles/` |
| Demo video | `public/cyberx-demo.mp4` |
| Live / SEO URLs | `index.html`, `public/sitemap.xml` |

---

## Related links

| Link | URL |
|------|-----|
| **Live website** | [https://cyberx.cyberwolf360.in/](https://cyberx.cyberwolf360.in/) |
| **Desktop product repo** | [github.com/Tamilselvan-S-Cyber-Security/Cyber-X](https://github.com/Tamilselvan-S-Cyber-Security/Cyber-X) |
| **Official release** | [releases/tag/CyberX](https://github.com/Tamilselvan-S-Cyber-Security/Cyber-X/releases/tag/CyberX) |
| **Sponsor** | [https://www.cyberwolf360.in](https://www.cyberwolf360.in) |
