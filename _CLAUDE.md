# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a personal portfolio website built with Jekyll and hosted on GitHub Pages. The site showcases Jonathan Gartland's professional experience, projects, and technical skills as a software engineer and senior QA engineer.

## Technology Stack

- **Static Site Generator:** Jekyll 3.9.3
- **Theme:** Minima 2.0 (with custom overrides)
- **Markdown Processor:** Kramdown with GFM parser
- **Hosting:** GitHub Pages
- **Plugins:**
  - jekyll-feed (RSS feed generation)
  - jemoji (emoji support)

## GitHub Pages Context

GitHub Pages publishes static content directly from a repository branch.

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

## Development Commands

### Local Development
```bash
# Install dependencies
bundle install

# Start local development server
bundle exec jekyll serve

# The site will be available at http://localhost:4000
# Changes to most files are automatically recompiled (except _config.yml)
```

For a plain static preview (no Jekyll build), you can use `npx serve` or `python -m http.server`.

### Important Notes
- **Configuration changes:** After modifying `_config.yml`, you must restart the Jekyll server for changes to take effect
- **Site generation:** Jekyll builds the site into the `_site/` directory (ignored by git)

## Site Architecture

### Content Structure

The site has three main content pages, each defined as a markdown file in the root:

1. **index.md** - Home page with personal introduction and photo
2. **experience.md** - Resume/CV page with professional experience and skills (permalink: `/experience/`)
3. **projects.md** - Portfolio of technical projects (permalink: `/projects/`)

### Directory Structure

- **_config.yml** - Jekyll site configuration (site metadata, build settings, theme configuration)
- **_includes/** - HTML partial templates for reusable components
  - Custom overrides for Minima theme (header.html, footer.html, head.html, etc.)
  - Social media icons in `social-icons/` subdirectory
  - Custom templates for social links, SVG symbols, analytics
- **_sass/** - Sass stylesheets
  - `minima/` contains theme customizations and overrides
  - Includes custom-styles.scss and custom-variables.scss for personalization
- **_posts/** - Blog posts (currently contains example posts, not actively used)
  - Posts follow Jekyll naming convention: `YYYY-MM-DD-title.md`
  - Posts use front matter with layout, title, date, categories, and tags
- **assets/** - Static assets
  - `css/` - Main stylesheet entry point
  - `minima-social-icons.liquid` - Social icon definitions
- **Root directory** - Contains large image files used in the site (JPG, PNG)

### Theme Customization

This site uses the Minima theme but overrides several components in `_includes/` to customize appearance and functionality. When modifying the site's look and feel:

- Check `_sass/minima/` for style customizations
- Check `_includes/` for template overrides
- The theme uses Sass variables defined in `_sass/minima/custom-variables.scss`

### Content Formatting

- **Markdown:** All content pages use GitHub-flavored Markdown
- **Front Matter:** Each page requires YAML front matter with `layout`, `title`, and `permalink`
- **Badges:** Experience and projects pages extensively use shields.io badges for technology logos
- **Images:** Large images are stored in the root directory and referenced directly

## Git Workflow

- **Main branch:** `main` - primary development branch
- **Current branch:** `gh-pages` - GitHub Pages deployment branch (currently checked out)
- **Modified files:** experience.md has uncommitted changes

When making commits, ensure changes are pushed to the appropriate branch for GitHub Pages deployment.

## Key Considerations

1. **GitHub Pages Compatibility:** This site is designed to work with GitHub Pages' Jekyll support. Avoid using plugins that aren't supported by GitHub Pages.

2. **Image Optimization:** The root directory contains several large JPG files (PXL_*.jpg files are 1.7MB-3.5MB). Consider optimizing these for web delivery if site performance becomes an issue.

3. **Badge URLs:** The experience.md and projects.md files contain many shields.io badge URLs. When updating technologies, maintain consistent badge styling (`style=for-the-badge`).

4. **Blog Posts:** The `_posts/` directory contains example posts but the blog functionality isn't actively used. The home page uses the `home` layout which typically displays posts, but the focus is on the static portfolio pages.
