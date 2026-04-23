# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static HTML marketing website for **Remote IDE**, an iPadOS app for SSH-based code editing on iPad. There is no build system, package manager, or test framework — the entire site is a single `index.html` file with embedded CSS and JavaScript.

## Development

To preview locally:
```bash
python3 -m http.server 8000
# then open http://localhost:8000
```

No build, lint, or test commands exist. The file is ready to serve as-is.

## Architecture

Single file: `index.html` (~906 lines)

- **CSS** (lines ~10–605): All styles are embedded in `<style>` tags. CSS custom properties define the color palette at the top (`--blue`, `--bg`, `--surface`, `--text`, `--muted`, `--green`). A subtle grid background is applied via a `::before` pseudo-element on `body`. Responsive breakpoint at 768px.
- **HTML structure** (lines ~603–889): Sections in order — nav → hero (with terminal code mockup) → features (9-card grid) → how-it-works (4-step flow) → tech-stack → privacy → support → footer.
- **JavaScript** (lines ~891–906): A single `IntersectionObserver` adds `.visible` to `.reveal` elements as they scroll into view, triggering CSS fade-up transitions. No other JS.

The page has no external JS dependencies — only Google Fonts (JetBrains Mono, DM Sans) are loaded externally.

## What This Site Describes

The page markets the actual Remote IDE iPadOS app (Swift/SwiftUI), which is **not** in this directory. The app uses: Runestone (syntax highlighting), SwiftTerm (terminal), Citadel (SSH/SFTP), keychain-swift (credentials), iCloud Drive (file sync).

## Original application path

/Users/sdidanov/Projects/Remote-IDE
