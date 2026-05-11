# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **Hugo** static site for **Remote IDE**, an iPadOS app for SSH-based code editing on iPad. It is deployed via Netlify.

## Development

```bash
hugo server          # dev server at http://localhost:1313
hugo build           # production build → public/
```

No npm, no Node.js, no test commands.

## Architecture

Hugo project at the repo root. Build output goes to `public/` (gitignored).

```
hugo.toml                  # Hugo config (baseURL, params, markup settings)
netlify.toml               # build command + publish dir for Netlify
static/
  css/main.css             # all styles (shared across all pages)
  fonts/                   # local woff2 fonts (DM Sans, JetBrains Mono)
  editor.svg               # hero image
  og-image.png
  robots.txt
layouts/
  _default/
    baseof.html            # base template: head, nav, main block, footer, scripts
    single.html            # fallback single page
    list.html              # fallback list page
  index.html               # home page (hero + features + privacy + support)
  features/
    single.html            # feature detail page layout
  blog/
    list.html              # blog listing
    single.html            # blog post
  partials/
    head.html              # <head>: meta, OG, schema.org (home only), CSS link
    nav.html               # fixed nav with logo and links
    footer.html            # footer
    scripts.html           # IntersectionObserver for .reveal animations
content/
  _index.md                # home page front matter
  features/
    _index.md
    multi-window.md        # Split View & Stage Manager feature page
  blog/
    _index.md
    getting-started.md     # first blog post
```

## CSS Custom Properties

Defined in `static/css/main.css` at `:root`:
- `--blue #007AFF`, `--blue-dim`, `--blue-glow`
- `--bg #0a0a0f`, `--bg2`, `--surface #13131e`
- `--border`, `--text #e8e8f0`, `--muted #7a7a96`
- `--green #30d158`, `--amber #ffd60a`
- `--mono` (JetBrains Mono), `--sans` (DM Sans)

Responsive breakpoint at 768px.

## Adding Content

**New blog post:** create `content/blog/my-post.md` with front matter:
```yaml
---
title: "Post Title"
date: 2026-05-10
description: "One-line summary shown as excerpt."
---
```

**New feature page:** create `content/features/my-feature.md` with:
```yaml
---
title: "Feature Name"
description: "Short description shown in page header."
icon: '<svg>...</svg>'
---
```
The layout in `layouts/features/single.html` renders the icon, title, description, `{{ .Content }}`, and a CTA box automatically.

## What This Site Describes

The page markets the actual Remote IDE iPadOS app (Swift/SwiftUI), which is **not** in this directory. The app uses: Runestone (syntax highlighting), SwiftTerm (terminal), Citadel (SSH/SFTP), keychain-swift (credentials), iCloud Drive (file sync).

## Original application path

/Users/sdidanov/Projects/Remote-IDE
