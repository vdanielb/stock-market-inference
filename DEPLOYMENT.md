# GitHub Pages Deployment Guide

This guide explains how to deploy the MkDocs site to GitHub Pages.

## Prerequisites

1. Install MkDocs and the Material theme:
```bash
pip install mkdocs mkdocs-material
```

## Local Testing

Before deploying, test the site locally:

```bash
mkdocs serve
```

This will start a local server (usually at `http://127.0.0.1:8000`) where you can preview the site.

## Deploy to GitHub Pages

### Option 1: Using mkdocs gh-deploy (Recommended)

This is the simplest method. It builds the site and deploys it to the `gh-pages` branch:

```bash
mkdocs gh-deploy
```

**Note**: Make sure you have:
- Git initialized in the repository
- A remote repository set up on GitHub
- Push permissions to the repository

### Option 2: Manual Deployment

1. Build the site:
```bash
mkdocs build
```

2. This creates a `site/` directory with the static HTML files.

3. Push the `site/` directory contents to the `gh-pages` branch on GitHub.

## GitHub Pages Configuration

After deployment, configure GitHub Pages in your repository settings:

1. Go to **Settings** → **Pages**
2. Under **Source**, select the `gh-pages` branch
3. Select the `/ (root)` folder
4. Click **Save**

Your site will be available at: `https://[username].github.io/[repository-name]`

## Updating the Site

Whenever you make changes to the documentation:

1. Update the markdown files in the `docs/` directory
2. Run `mkdocs gh-deploy` again
3. The changes will be live within a few minutes
