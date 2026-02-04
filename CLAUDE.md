# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a GitHub Pages personal site repository (jonathan-gartland.github.io). The project is newly initialized and does not yet have a build system or framework in place.

## GitHub Pages Context

GitHub Pages is a static site hosting service that publishes web content directly from a GitHub repository.

### Supported Technologies
- **Jekyll**: Built-in support for Jekyll static site generator (recommended for GitHub Pages)
- **Static HTML/CSS/JS**: Plain static files work without any build system
- **Custom GitHub Actions**: For other static site generators (Hugo, Eleventy, Next.js static export, etc.)

### Configuration Options
- **Publishing source**: Configure which branch/folder to publish from (typically `main` branch or `/docs` folder)
- **Custom domains**: Can use custom domain instead of `username.github.io`
- **HTTPS**: Enforced by default for security
- **Custom 404 pages**: Create a `404.html` or `404.md` file

### Key Files
- `_config.yml`: Jekyll configuration (if using Jekyll)
- `index.html` or `index.md`: Site entry point
- `404.html`: Custom error page
- `CNAME`: Custom domain configuration (if applicable)

## Deployment

The site is deployed automatically via GitHub Pages when changes are pushed to the main branch.

### Deployment Options
1. **Direct push**: Changes to main branch auto-deploy
2. **GitHub Actions**: Custom workflows for build steps (use `peaceiris/actions-gh-pages` or similar)

### Local Testing
- Jekyll sites: `bundle exec jekyll serve`
- Static sites: Use any local server (e.g., `npx serve` or `python -m http.server`)
