# WARP.md

This file provides guidance to WARP (warp.dev) when working with code in this repository.

## Project Overview

This is eggy0223's personal "About Me" website featuring a red-orange gradient theme with gaming interests and social links. It's a simple static HTML/CSS website with glassmorphism UI effects and responsive design.

## Architecture & Structure

- **Single-page static website**: No build system or frameworks required
- **Core files**:
  - `index.html`: Main HTML structure with semantic sections (header, about-me, interests, links, footer)
  - `styles.css`: Complete styling with CSS custom properties, animations, and responsive breakpoints
  - `README.md`: Project documentation and feature overview

## Development Commands

### Local Development
```bash
# Simply open the HTML file in any modern browser
start index.html

# Or serve locally using Python (if available)
python -m http.server 8000

# Or using Node.js live-server (if installed)
npx live-server
```

### Version Control
```bash
# Check current status
git status

# Add and commit changes
git add .
git commit -m "Update: description of changes"

# View recent commits
git log --oneline -10
```

## Key Design Patterns

### CSS Architecture
- **CSS Custom Properties**: Uses `:root` variables for consistent theming (`--primary-red`, `--primary-orange`, etc.)
- **Glassmorphism Effects**: Sections use `backdrop-filter: blur(10px)` with semi-transparent backgrounds
- **Responsive Grid Layout**: Interest list uses CSS Grid with `auto-fit` and `minmax()` for responsive behavior
- **Animation System**: Keyframe animations for glow effects on the main heading

### Content Structure
- **Gaming-focused personal branding**: Reflects autism-positive language and gaming interests
- **Hyperfixation tracking**: Current interests section designed to be easily updated
- **Social integration**: Roblox profile link and Discord username display

## Common Development Tasks

### Updating Content
- **Interests/Hyperfixations**: Modify the `<ul class="interest-list">` in `index.html`
- **Social Links**: Update links in the `.social-links` section
- **About Me section**: Edit the personal description paragraph

### Styling Changes
- **Theme colors**: Modify CSS custom properties in `:root`
- **Fonts**: Currently uses Google Fonts (Metal Mania, Nosifer, Georgia)
- **Responsive breakpoints**: Media queries at 768px and 480px

### Testing Responsiveness
```bash
# Test different viewport sizes in browser dev tools
# Key breakpoints: 768px (tablet), 480px (mobile)
```

## Project Context

This website was created as a personal project "made with ❤️ for a friend" and serves as eggy0223's online presence showcasing gaming interests and providing social contact information. The design emphasizes accessibility and personal expression with autism-positive language and gaming culture references.