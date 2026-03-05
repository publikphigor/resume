# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Static resume/portfolio website for Koladele Olaitan (Senior Frontend Engineer). Single-page HTML site hosted on Netlify at https://koladele-resume.netlify.app/.

## Architecture

- **Single file site**: All content, styling, and structure live in `index.html` (inline CSS in `<style>`, no external stylesheets or JS besides Ionicons)
- **PDF resume**: `Koladele-Olaitan_Resume.pdf` is served via a download button
- **Icons**: Uses Ionicons 5.5.2 loaded from unpkg CDN
- **Fonts**: Google Fonts (Raleway)
- **No build step**: Pure static HTML — open `index.html` directly or use VS Code Live Server (configured on port 5501 in `.vscode/settings.json`)

## Development

To preview locally, use VS Code Live Server extension or any static file server. No dependencies to install.

## Key Conventions

- Resume content changes go directly in `index.html` — there is no templating or data layer
- When updating resume content, also update the PDF file to keep them in sync
- CSS uses a mobile breakpoint at 640px with flexbox/grid layout
- Link color is `#0072b1`; body text is `#262626`; secondary text is `#4c4c4c`
