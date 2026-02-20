# Academic Portfolio Website

A clean, fast, and responsive academic portfolio website built with **Jekyll** and deployed on **GitHub Pages**.  
This repository contains the source code and content for my personal website (publications, projects, CV, and updates).

## Live Site
- Website: https://YOUR_USERNAME.github.io/ (or your custom domain)

## What’s Included
- **Home**: short bio + highlights
- **Publications**: BibTeX-driven list with optional links (PDF, code, DOI, arXiv, etc.)
- **Projects**: featured work with images and descriptions
- **CV**: YAML/JSON-based CV page (depending on configuration)
- **News/Updates**: lightweight posts for announcements
- **Responsive design**: works well on desktop and mobile
- **Light/Dark mode** (theme-dependent)

## Repository Structure (Quick Map)
- `_pages/` → main pages (about, publications, projects, cv, etc.)
- `_posts/` → blog posts (optional)
- `_news/` → short updates shown on the homepage (if enabled)
- `_projects/` → project entries displayed as a grid
- `_bibliography/` → BibTeX files for publications
- `_data/` → structured data (CV, settings, etc.)
- `assets/` → images, PDFs, and other static files
- `_config.yml` → site configuration

## Update Content
### 1) Profile + Site Info
Edit:
- `_config.yml` (name, description, social links, analytics)
- `about.md` or `_pages/about.md` (bio, photo, research interests)

### 2) Publications
Edit:
- `_bibliography/papers.bib`

Optional: attach files in `assets/pdf/` and reference them from BibTeX entries.

### 3) Projects
Add files in:
- `_projects/`

Each project is a Markdown file with front matter (title, description, image, tags).

### 4) CV
Depending on your setup, update one of:
- `_data/cv.yml` (YAML CV)
- `assets/json/resume.json` (JSONResume)

## Local Development
Requirements: Ruby + Bundler

```bash
bundle install
bundle exec jekyll serve
