# Aalok Tiwari — personal website

A static, multi-page academic site (About, Research, Publications, Talks & Posters).
Plain HTML + CSS, no build step. Deploys to GitHub Pages as-is.

```
index.html          About / bio + contact + CV link
research.html       Research themes
publications.html   Papers & preprints
talks.html          Talks & posters (slide/poster links)
assets/
  style.css         Shared styling (academic minimalist)
  Aalok_Tiwari_CV.pdf   <- add your compiled CV here
  photo.jpg             <- optional headshot (see index.html)
  slides/               <- drop talk slides / poster PDFs here
.nojekyll           Tells GitHub Pages to serve files as-is
```

## Deploy to GitHub Pages

### Option A — personal site at `https://<username>.github.io` (recommended)

1. Create a new **public** repo named exactly `<username>.github.io`
   (e.g. `aalok-tiwari.github.io`).
2. Put the contents of this folder in the repo root, then push:
   ```bash
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/<username>/<username>.github.io.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   branch `main`, folder `/ (root)`, then **Save**.
4. Your site goes live at `https://<username>.github.io` within a minute or two.

### Option B — project site at `https://<username>.github.io/<repo>`

Same as above, but name the repo anything (e.g. `website`). The site URL will include
the repo name. All links here are relative, so it works either way with no changes.

## Before you publish — quick checklist

- [ ] Add your compiled CV as `assets/Aalok_Tiwari_CV.pdf`
- [ ] (Optional) add `assets/photo.jpg` and uncomment the `<img>` line in `index.html`
- [ ] Add any slide/poster PDFs to `assets/slides/` (filenames already referenced in `talks.html`)
- [ ] Add your GitHub link to the contact row in `index.html` if you'd like
- [ ] Skim the publication author lists and DOIs

## Custom domain (optional)

Add a file named `CNAME` containing your domain (e.g. `aaloktiwari.com`), then set the
DNS records per GitHub's guide: https://docs.github.com/pages/configuring-a-custom-domain-for-your-github-pages-site

## Editing

Everything is hand-editable HTML. Colors, fonts, and spacing live in `assets/style.css`
(the accent color is the `--accent` variable near the top).
