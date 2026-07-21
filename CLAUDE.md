# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this is

M. Cecilia Ramírez-Michelena's personal academic/job-market site, deployed via GitHub Pages at `mcramirezmichelena.github.io`. It is a **hand-authored static site** — a single `index.html` plus vendored `css/` and `js/` from the "Source Themes Academic v4.8.0" builder (Bootstrap-based). There is no build step, no Jekyll, no package manager, and no `_config.yml` — everything ships as-is.

## Working with this repo

- All page content (Biography, Research, Policy & Practice, Teaching, Contact) lives directly in `index.html`. There are no separate markdown source files or content collections — edit the HTML in place.
- `css/academic.css` and `js/academic.min.js` are vendored template assets (theme + Bootstrap). Don't hand-edit them; page-specific style tweaks (`.dept-line`, `.edu-uni`, `.edu-date`, heading accents, dark-mode overrides, etc.) go in the `<style>` block inside `index.html`'s `<head>`.
- No build/lint/test commands exist — there's nothing to compile. To preview, open `index.html` directly in a browser or serve the folder with any static file server.
- Static assets: CVs in `assets/cv/`, working papers in `assets/papers/`, profile photo in `assets/img/`.

## Deploy

- Branch `main` is the live branch tracked by GitHub Pages (`origin` remote). Branch `master`, if present, is an old unused template branch — ignore it.
- Pushing to `origin/main` deploys immediately to the live site. Always confirm with the user before pushing (per standard git safety practice for this repo) — committing locally first is fine and expected.

## Session-to-session tracking

- `Website - cambios pendientes.md` (Spanish) is a running TODO note the user maintains across sessions for undecided/pending items (pending deploys, unresolved image placement, open questions on paper dates, etc.). Check it at the start of a session for open threads, and update it when pending items are resolved or new ones come up.
