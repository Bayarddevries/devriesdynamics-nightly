# devriesdynamics-nightly — Bayard deVries Portfolio

**Status:** Active, deployed
**Live site:** https://bayarddevries.github.io/devriesdynamics-nightly/
**Platform:** Static HTML/CSS/JS (vanilla, no build step)

---

## Overview

Professional portfolio website for **Bayard deVries** — 15+ years of
ops and project leadership, Métis heritage projects, and interactive
design. The site showcases professional experience, heritage projects,
and technical capabilities.

## Pages

| Page | Description |
|------|-------------|
| `index.html` | Hero + stats bar + CTA |
| `projects.html` | 4 featured projects with detail modals |
| `about.html` | About / design philosophy |
| `resume.html` | Resume / CV |
| `design.html` | Design showcase (if enabled) |

## Featured Projects

1. **Shoebox V2** — Red River Métis Digital Archive (React/TS)
2. **Homeland Map** — Interactive Métis historical map (Leaflet)
3. **Métis Trail RPG** — Tabletop fur trader RPG (Godot)
4. **RRMNHC Site** — Heritage Centre website (static)

## Design System

- **Theme:** Dark forest (#131A0F) + brass (#C49A3A) + cream (#F5F0E8)
- **Fonts:** Space Grotesk (headings), DM Sans (body) via Google Fonts
- **Effects:** Animated particle background, hover card animations
- **Responsive:** Mobile-first, all vanilla CSS
- **No build step:** Pure HTML/CSS/JS served directly from `nightly` branch

## Architecture

```
devriesdynamics-nightly/
├── index.html          # Homepage
├── projects.html       # Project cards + detail modals
├── about.html          # About page
├── resume.html         # Resume/CV
├── design.html         # Design showcase
├── styles.css          # All styles (design tokens + components)
├── script.js           # Interactions (modals, particles, nav)
├── 404.html            # Custom 404
├── assets/             # Images, graphics
├── .github/            # GitHub Actions (Pages deploy)
├── CHANGELOG.md        # Full project history
└── STATUS.md           # Current project status
```

## Deployment

Auto-deploys to GitHub Pages on push to `nightly` branch.
Workflow: `.github/workflows/` → Pages build → live site.

## CHANGELOG & STATUS

See `CHANGELOG.md` for full development history and
`STATUS.md` for current project state.
