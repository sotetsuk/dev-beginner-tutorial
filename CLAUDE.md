# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a beginner development tutorial website built with MkDocs Material. The tutorial is in Japanese and teaches fundamental software development skills including UNIX commands, Python, Git/GitHub, and C++.

## Commands

### Local Development
```bash
# Start local server with auto-refresh (requires Docker)
./serve.sh
# Server runs at http://0.0.0.0:8000/
```

### Build & Deploy
```bash
# Install dependencies
pip install mkdocs-material

# Deploy to GitHub Pages (CI automatically does this on main branch push)
mkdocs gh-deploy --force
```

## Architecture

- **MkDocs Material**: Static site generator for documentation
- **Docker**: Used for local development environment via `serve.sh`
- **GitHub Actions**: Automatic deployment to GitHub Pages on push to main branch
- **Content Structure**: Tutorial pages in `docs/` directory, each covering different development topics
- **Configuration**: Site settings in `mkdocs.yml` including navigation, theme, and markdown extensions