# Hybrid Static Site Starter

A one-page, section-based personal+professional site (punk/activist vibes) for GitHub Pages.

## Files
- `index.html` — the page content. Replace ALL CAPS placeholders with your details.
- `style.css` — styles.
- `.nojekyll` — ensures GitHub Pages doesn’t try to process Jekyll.
- `README.md` — this guide.

## Quick Start (no terminal)
1. Create a public repo named **YOUR-USERNAME.github.io** on GitHub.
2. Click *Add file → Upload files* and upload **all** files from this folder.
3. Go to *Settings → Pages* and set Source = *Deploy from a branch*, Branch = *main*, Folder = */ (root)*.
4. Your site will be at https://YOUR-USERNAME.github.io

## Quick Start (automated via GitHub CLI)
If you use the `gh` CLI and have logged in (`gh auth login`):

```bash
# 1) Set your GitHub username
USER=yourusername

# 2) Create the repo
gh repo create "$USER/$USER.github.io" --public --confirm

# 3) Clone and populate
git clone "https://github.com/$USER/$USER.github.io"
cd "$USER.github.io"

# Copy the starter files into this folder (adjust path):
# (Assuming you downloaded and unzipped to ~/Downloads/hybrid_site_starter)
cp -R ~/Downloads/hybrid_site_starter/* .

# 4) Commit & push
git add .
git commit -m "Initial site"
git branch -M main
git push -u origin main

# 5) Enable Pages (user/organization site usually goes live automatically on push)
# If needed, toggle in Settings → Pages manually.
```

## Custom Domain (optional)
Point your domain’s DNS to GitHub Pages and set the custom domain in *Settings → Pages*.
