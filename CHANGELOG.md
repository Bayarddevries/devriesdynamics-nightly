# CHANGELOG

All notable changes to the devriesdynamics.com portfolio site will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## [Unreleased]

### Added
- Developer notes section in projects.html with fix summary and testing instructions
- Comprehensive CHANGELOG.md for all agents to understand project history

## [2024-05-09] - Fixed Projects Modal and Card Rendering

### Changed
- **Projects Modal Fix**: Replaced event delegation with inline `onclick="openModal(i)"` approach to prevent rendering failures
- **DOM Readiness**: Ensured `DOMContentLoaded` wrapper for `renderCards()` function call
- **Safety Fallback**: Added `setTimeout` fallback to trigger `renderCards()` if initial render fails after 1 second
- **Debug Logging**: Added `console.log("Rendering cards...")` to track render function execution

### Technical Details
- **Issue**: Project cards were rendering but modal clicks were not working due to event delegation conflicts
- **Attempted Solution**: Event delegation via `cardsContainer.addEventListener` (caused total rendering failure)
- **Final Solution**: Inline onclick per project card with DOMContentLoaded wrapper
- **Projects Array**: Maintains 4 entries (Shoebox V2, Homeland Map, Métis Trail RPG, RRMNHC Site)
- **Modal Features**: Full-screen overlay with project details, navigation arrows, keyboard support (Escape/Arrow keys)

### Files Modified
- `projects.html` - Fixed modal click handling and added developer documentation
- `styles.css` - No changes (dark forest + brass theme maintained)

### Testing Notes
- Reload Projects page and check console for "Rendering cards..." message
- Click any project card should open modal with full details
- Modal navigation: Use arrow keys or close button to exit

---

## [2024-05-09] - Portfolio Site Completion

### Added
- Portfolio site with dark forest + brass theme (Space Grotesk + DM Sans fonts)
- Homepage with hero, project cards, and contact information
- Projects page with interactive cards and modal details
- Resume page with downloadable Google Drive link
- Custom 404 page with dark theme
- Design system page with color palette and shader demos (private/unlinked)

### Features
- 4 project cards with live links and screenshots
- Fully responsive design
- Keyboard navigation support
- Animated CSS background on Projects page
- Stats bar with brass accent numbers
- Contact footer with "Site by Bayard" attribution

### Deployed
- GitHub Pages: https://bayarddevries.github.io/devriesdynamics-nightly/
- Branch: nightly
- Auto-deploys on push to main branch