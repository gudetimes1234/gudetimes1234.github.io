# Personal Site

A minimal personal website and blog built with Jekyll and the Tale theme.

## Setup

This site uses Jekyll with the Tale remote theme. To run locally:

```bash
bundle install
bundle exec jekyll serve
```

Visit `http://localhost:4000` to preview the site.

## Customisation

- **Site info**: Edit `_config.yml` to update your name, bio, and social links
- **Landing page**: Edit `index.md`
- **Styles**: Add custom CSS to `assets/custom.css`

## Writing Posts

Create markdown files in `_posts/` with the naming format: `YYYY-MM-DD-title.md`

Example post:

```markdown
---
layout: post
title: "My First Post"
date: 2026-01-24
---

Your content here...
```

## Deployment

This site is automatically deployed to GitHub Pages when you push to the `master` branch.
