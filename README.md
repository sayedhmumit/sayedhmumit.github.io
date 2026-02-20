# sayedhmumit.github.io

Source code for my personal academic website, hosted on GitHub Pages.

**Live site:** https://sayedhmumit.github.io

## Overview
This repository contains the content and configuration for my portfolio website, including:
- Research interests and short bio
- Publications (BibTeX-driven, if enabled)
- Projects and selected work
- CV / Resume page
- News or updates (optional)
- Blog posts (optional)

## Tech Stack
- **Jekyll** (static site generator)
- **GitHub Pages** (deployment/hosting)
- Theme: **al-folio** (customized)

## Repository Layout (Typical)
Your repo may not include all of these folders, but most al-folio setups follow this pattern:

- `_pages/` → main pages (about, publications, projects, cv)
- `_projects/` → project entries
- `_news/` → short updates (shown on homepage if enabled)
- `_posts/` → blog posts (optional)
- `_bibliography/` → BibTeX files for publications (optional)
- `_data/` → structured data (CV YAML, settings)
- `assets/` → images, PDFs, files
- `_config.yml` → site configuration

## How to Update Content
### Profile + Links
Edit `_config.yml` and your about page (commonly `_pages/about.md` or similar).

### Publications
If enabled, update your BibTeX in `_bibliography/` (often `papers.bib`).

### Projects
Add or edit Markdown files in `_projects/`.

### CV
Depending on your setup, update one of:
- `_data/cv.yml`
- `assets/json/resume.json`

## Run Locally
Requirements: Ruby + Bundler.

```bash
bundle install
bundle exec jekyll serve
