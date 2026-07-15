# TechFest 2026 Website — GitHub Pages Deployment Guide

This folder is ready to publish with **GitHub Pages** (100% free). Follow these steps:

## 1. Create a new GitHub repository
- Go to https://github.com/new
- Name it anything, e.g. `techfest2026`
- Set it to **Public** (required for free GitHub Pages)
- Don't initialize with a README (you already have files)
- Click **Create repository**

## 2. Upload these files
**Option A — Drag and drop (easiest, no terminal needed):**
- On your new repo's page, click **"uploading an existing file"**
- Drag ALL the files/folders from this zip (index.html, css/, images/, videos/, audio/, *.html) directly in
- Scroll down, click **Commit changes**

**Option B — Git command line:**
```bash
cd path/to/this/extracted/folder
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
git push -u origin main
```

## 3. Turn on GitHub Pages
- In your repo, go to **Settings → Pages** (left sidebar)
- Under "Build and deployment" → Source, select **Deploy from a branch**
- Branch: **main**, folder: **/ (root)**
- Click **Save**

## 4. Visit your site
- Wait 1-2 minutes, then your site will be live at:
  `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`
- GitHub will also show this URL at the top of the Pages settings page once it's ready

## Notes
- `index.html` is your homepage — GitHub Pages automatically serves it at the root URL.
- All internal links (nav bar, images, videos, audio) use relative paths, so nothing needs to change.
- Total site size: ~60MB, well within GitHub's free limits.
- If you ever want a custom domain (like techfest2026.com) instead of the default `github.io` address, that requires buying a domain (~$10-15/year) — GitHub Pages itself stays free either way.
