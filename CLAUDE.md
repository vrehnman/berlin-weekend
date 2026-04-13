# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project overview

Static site for a Berlin Kreuzberg weekend trip plan (in Swedish). Single-page HTML with no build step, no dependencies, no frameworks.

## Architecture

- `index.html` – The entire site. Self-contained HTML/CSS, no JavaScript dependencies.
- `kreuzberg-weekend.md` – Markdown version of the same content for sharing.
- `.gitattributes` – Set to `* -text` to disable all LF/CRLF conversion.

## Deployment

Deployed to GitHub Pages via GitHub Actions on push to `master`. The workflow uploads the repo root directly — no build step.

- Branch: `master` (not `main`)
- To deploy: just push to `master`
- Manual trigger: Actions → "Deploy to GitHub Pages" → Run workflow

## Development

Open `index.html` in a browser. No server needed.
