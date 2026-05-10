---
title: Project Status
date: 2024-05-09
status: Active
version: v1.0.0
branch: nightly
deploy_url: https://bayarddevries.github.io/devriesdynamics-nightly/
---

# devriesdynamics.com Portfolio Site

## Project Overview
Professional portfolio website for Bayard deVries featuring 15+ year ops leadership career, Métis heritage projects, and interactive design elements.

## Current Status
✅ **Complete and deployed** - All core functionality working as of 2024-05-09

## Key Features
- **Design System**: Dark forest (#131A0F) + brass (#C49A3A) theme with Space Grotesk + DM Sans typography
- **Interactive Elements**: Hover card effects, animated backgrounds, modals with keyboard navigation
- **4 Projects**: Shoebox V2, Homeland Map, Métis Trail RPG, RRMNHC Site with live links
- **Responsive Design**: Mobile-first approach with proper viewport handling
- **Accessibility**: Semantic HTML5, keyboard navigation, proper contrast ratios

## Technical Stack
- **Frontend**: HTML5, CSS3 (vanilla), vanilla JavaScript
- **Deployment**: GitHub Pages (nightly branch)
- **Fonts**: Google Fonts (Space Grotesk, DM Sans)
- **Icons**: Unicode symbols (×, ‹, ›)
- **Maps**: Leaflet integration (Homeland Map project)

## Recent Fixes
- **Projects Modal**: Fixed click handling using inline onclick approach
- **Rendering**: Added DOMContentLoaded wrapper and safety fallback
- **Debug**: Console logging for troubleshooting

## Project Structure
```
devriesdynamics.com/
├── index.html          # Homepage with hero and project overview
├── projects.html       # Interactive cards with modal details
├── resume.html         # Resume page with Google Drive download
├── 404.html           # Custom error page
├── design.html        # Design system (private, not linked)
├── styles.css         # Shared styles and theme variables
├── assets/            # Screenshots and media
├── CHANGELOG.md       # Version history
└── README.md          # This status file
```

## Maintenance Notes
- **Auto-deploys**: Commits to main branch trigger GitHub Pages deployment
- **Design Page**: Not linked in navigation (private playground)
- **Nightly Branch**: All changes deployed automatically to GitHub Pages
- **Cron Jobs**: nightly-tinkering job is paused (2024-05-09)

## TODO
- DNS/CNAME setup for custom domain (devriesdynamics.com)
- Additional project screenshots as they're completed
- Performance optimization (current: ~1.5KB CSS, ~8KB JS)

---

**Last Updated**: 2024-05-09 by Hermes Agent