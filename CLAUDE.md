# Aalok Tiwari — Personal Website

Static HTML/CSS academic personal website, hosted on **GitHub Pages** at https://aaloktrii.github.io/.

## Stack

Plain HTML + CSS, zero build step. No frameworks, no bundler.
- `index.html` — About / landing
- `research.html` — Research narrative, expertise, conferences, awards
- `publications.html` — Full publication list
- `outreach.html` — Teaching, outreach, leadership
- `assets/style.css` — All styles (IBM Plex Mono, CSS variables for light/dark)
- `assets/theme.js` — Light/dark toggle

## Git workflow

After every edit, **always commit and push**:

```bash
git add <changed files>
git commit -m "short description"
git push origin main
```

GitHub Pages deploys automatically from `main` within ~1 minute. No CI or build step needed.

## Conventions

- Publications: title is the clickable link (arXiv or DOI). Full author list. Bold **A. Tiwari**. Equal contributions marked with `*`. Papers without a public link are HTML-commented out (`<!-- hidden until link available: ... -->`).
- Dates: use en-dash (`&ndash;`) for ranges.
- Subscripts/superscripts: use `<sub>`/`<sup>` HTML tags.
- Keep all styles in `assets/style.css`; no inline styles except the occasional `color: inherit` on links that must inherit text color.
