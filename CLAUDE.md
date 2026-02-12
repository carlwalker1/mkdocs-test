# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Jekyll-based static website configured for GitHub Pages deployment. Content is written in Markdown and automatically built/deployed when pushed to the main branch.

## Development Commands

**Local Preview:**
```bash
jekyll serve
```
Site runs at `http://localhost:4000`. Jekyll watches for file changes and rebuilds automatically.

**First-time Setup (if needed):**
```bash
gem install jekyll bundler
bundle install
```

## Architecture

- **Content**: Markdown files (`.md`) with YAML front matter define pages
- **Configuration**: `_config.yml` contains site settings, theme, and build configuration
- **Theme**: Uses GitHub Pages Primer theme (`pages-themes/primer@v0.6.0`) via `remote_theme`
- **Markdown Processor**: Kramdown (specified in `_config.yml`)
- **Build Output**: Jekyll generates static HTML in `_site/` directory (git-ignored)

## Key Configuration

**Theme Configuration** (`_config.yml`):
- Current theme: `remote_theme: pages-themes/primer@v0.6.0`
- Changing themes requires updating the `remote_theme` value and ensuring `jekyll-remote-theme` plugin is listed

**Base URL**:
- Currently set to `baseurl: ""` for root-level hosting
- For repository-based GitHub Pages (e.g., `username.github.io/repo-name/`), set `baseurl: "/repo-name"`

## Content Editing

- Edit `index.md` for homepage content
- Create new `.md` files for additional pages
- All Markdown files must include YAML front matter (at minimum: `layout: default`)
- Kramdown Markdown features are supported (tables, code blocks with syntax highlighting, etc.)

## Deployment

GitHub Pages automatically builds and deploys on push to main branch. No manual build step required for production.
