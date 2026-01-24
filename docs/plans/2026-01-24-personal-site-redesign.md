# Personal Site Redesign with Tale Theme

**Date:** 2026-01-24

## Overview

Rebuild personal GitHub Pages site using Tale - a minimal Jekyll theme. The site will feature a clean landing page with bio and social links, plus blog infrastructure ready for future posts.

## Project Structure

```
gudetimes1234.github.io/
├── _config.yml              # Jekyll and Tale configuration
├── _posts/                  # Blog posts (empty initially)
├── assets/
│   └── custom.css          # Style overrides
├── index.md                # Landing page content
├── blog.md                 # Blog listing page
├── Gemfile                 # Ruby dependencies
└── README.md               # Updated project docs
```

## Technical Approach

### Remote Theme Strategy

Use Tale as a Jekyll remote theme rather than forking. Benefits:
- Clean repository with only content and customisations
- Automatic theme updates
- Easier maintenance

Configuration in `_config.yml` points to `chesterhow/tale` repository.

### Landing Page

Simple landing page (`index.md`) containing:
- Name as heading
- Brief bio (1-2 sentences)
- Social links (GitHub and LinkedIn)

Uses Tale's default layout with custom content.

### Blog Setup

Separate blog page (`blog.md`) that:
- Lists all posts chronologically (newest first)
- Uses Tale's built-in post archive layout
- Shows empty state when no posts exist

Blog posts go in `_posts/` folder using Jekyll naming: `YYYY-MM-DD-title.md`

### Navigation

Two-item navigation in header:
- Home → `/`
- Blog → `/blog`

Defined in `_config.yml`, rendered by Tale's layout.

### Customisation

`assets/custom.css` file ready for future style tweaks without modifying theme files. Starts empty, using Tale's default minimal black and white aesthetic.

## Post Format

Blog posts use standard Jekyll front matter:

```markdown
---
layout: post
title: "Post Title"
date: YYYY-MM-DD
---

Content in markdown...
```

## Configuration Details

Key `_config.yml` settings:
- Remote theme: `chesterhow/tale`
- Site name and bio
- Social links (GitHub, LinkedIn)
- Navigation items
- Permalink structure: `/blog/:year/:month/:day/:title`

## Implementation Notes

- Remove existing Semantic UI assets
- Keep repository focused on content
- Tale handles all theming and layout
- GitHub Pages builds automatically on push
