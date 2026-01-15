# Archetech Website - AI Coding Instructions

## Project Overview
This is a **static website** for Archetech (www.archetech.com) hosted on GitHub Pages via this repository. The site is hand-written HTML without frameworks, build tools, or dependencies.

**Key fact**: Changes pushed to `origin master` go live automatically in ~10 minutes.

## Architecture
- **index.html**: Landing page with company tagline and logo
- **Director_Bios.html**: Team member profiles and background information
- **logo.png, cs.png, dmc.png**: Image assets referenced in HTML
- **CNAME**: GitHub Pages configuration pointing to www.archetech.com

No build process, bundler, or static site generator—just plain HTML and CSS.

## Development Workflow
1. **Make changes** to `.html` files directly
2. **Test locally** by opening HTML files in a browser
3. **Commit and push** to master branch
4. **Deploy**: Changes appear live automatically (~10 minutes)

## Common Patterns & Conventions

### HTML Structure
- **Inline CSS** in `<style>` tags (no external stylesheets)
- **Absolute positioning** for layout (logo uses `position: absolute; top/left; margin` offsets)
- **Inline styles** on elements via `style` attributes (common in Director_Bios.html)
- **No semantic HTML5 elements**—uses generic `<div>`, `<table>`, `<p>` tags

### Styling Approach
- Heavy use of CSS positioning with pixel-based margins
- Hardcoded widths/heights (e.g., `height: 71%`, `width: 75%`)
- No responsive design—fixed layout without media queries
- Link styling defined globally in CSS (black color, no underline)

## Content Updates
- **Director bios**: Edit table structures in Director_Bios.html with director name, title, contact, and bio paragraphs
- **Landing page text**: Update tagline in `<p id="text">` on index.html
- **Images**: Place in repo root, reference by filename in `src` attributes
- **Links**: Use relative paths (`<a href="/Director_Bios.html">`, `<a href="/">`)

## Things to Avoid
- Don't introduce frameworks, build tools, or package managers
- Don't use external stylesheets or CDNs
- Don't refactor to semantic HTML or modern practices unless explicitly requested—this site works as-is
- Don't add version control for image assets (they should stay in repo)

## Quick Reference
- **Live site**: www.archetech.com
- **Source repo**: archetech.github.io
- **Deploy time**: ~10 minutes after push to master
- **Contact emails**: christian@archetech.com, david@archetech.com (in bios)
