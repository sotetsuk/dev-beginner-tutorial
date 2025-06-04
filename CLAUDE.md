# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a beginner development tutorial website built with MkDocs Material. The tutorial is in Japanese and teaches fundamental software development skills including UNIX commands, Python, Git/GitHub, and C++.

## Commands

### Local Development
```bash
# Start local server with auto-refresh (uses uvx to run mkdocs-material)
./serve.sh
# Server runs at http://127.0.0.1:8000/
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
- **uvx**: Tool runner from uv, used to run mkdocs-material without project setup
- **GitHub Actions**: Automatic deployment to GitHub Pages on push to main branch
- **Content Structure**: Tutorial pages in `docs/` directory, each covering different development topics
- **Configuration**: Site settings in `mkdocs.yml` including navigation, theme, and markdown extensions