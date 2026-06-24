# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is the documentation website for Vixen Lights software — a Hugo static site using the [Docsy](https://www.docsy.dev/) theme. Hugo modules (Go) manage the theme; npm manages CSS tooling (PostCSS/Autoprefixer).

## Common Commands

```sh
# Install JS dependencies (required before building)
npm install

# Update Hugo modules (Go-based theme dependencies)
hugo mod get -u

# Local dev server (auto-reloads on change)
hugo server

# Build for a specific environment
hugo --environment production   # outputs to public/
hugo --environment staging

# Tidy Go module cache
hugo mod tidy
```

There are no test commands — content correctness is verified by running `hugo server` and viewing the site.

## Architecture

### Configuration layering (`config/`)
Hugo uses environment-specific config merging:
- `config/_default/config.toml` — base config (baseURL set to `localhost:1313`, GA test ID, all feature flags)
- `config/production/` — overrides baseURL to `https://www.vixenlights.com/` and sets real GA/services
- `config/staging/` — overrides baseURL to `https://webtest.vixenlights.com/`

Run `hugo --environment production` (or `staging`) to activate the corresponding overlay.

### Content (`content/en/`)
All content lives under the `en/` language directory. Main sections: `docs/`, `download/`, `developer/`, `about/`, `community/`. Each section uses `_index.md` or `_index.html` for its landing page.

### Release data (`data/release/`)
The download pages are driven by GitHub API data stored in `data/release/latest.json` and `data/release/all.json`. In CI, these are fetched live from the `vixenlights/vixen` GitHub releases API before the build. For local development, these files must be present — update them manually or via `gh api /repos/vixenlights/vixen/releases/latest > data/release/latest.json`.

### Custom shortcodes (`layouts/shortcodes/`)
- `release-latest.html` — renders the latest Vixen release download card from `data/release/latest.json`
- `release-all.html` — renders all releases from `data/release/all.json`
- `download-img.html`, `video.html`, `figure.html`, `devbuild-first.html` — utility shortcodes
- `blocks/feature-release.html` — block-level shortcode for homepage feature sections

### Custom partials (`layouts/partials/`)
- `feedback.html`, `page-meta-links.html` — override Docsy defaults

### CI/CD (`.github/workflows/`)
- Push to `master` → builds with `production` environment → Docker image `vixenlights/www.vixenlights.com`
- Push to `develop` → builds with `staging` environment → Docker image `vixenlights/webtest.vixenlights.com`
- The build fetches fresh release JSON, runs `npm ci`, then `hugo --environment <env>`
- Final artifact is a Docker image (`nginx:stable` serving the `public/` directory) pushed to GHCR, then a Watchtower webhook triggers an auto-deploy
