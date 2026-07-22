# MINATAVR — site

Static two-page site: `index.html` (главная) + `strength.html` («Стать сильнее»).

## Files
- `index.html` — home page (renamed from `minatavr-prototype (70).html`)
- `strength.html` — strength page (renamed from `strength (7.2).html`)
- `*.webp` — image assets (must be added, see below)
- `.nojekyll` — disables Jekyll processing on GitHub Pages

## Links between pages
- Home → card «Стать сильнее» → CTA «Смотреть форматы» → `strength.html`
- strength.html → logo MINATAVR → `index.html`
- strength.html → nav item «Главная» (desktop + burger) → `index.html`
- In-page anchors on strength.html: `#formats`, `#approach`, `#result-system`, `#how-to-start`
- External links kept: Telegram (`https://t.me/CtereoC`, `https://t.me/Wolwar93`), Google Fonts

All internal paths are relative (no leading `/`, no `<base>`), so the site works from a
repo subpath on GitHub Pages.

## Required images (MISSING — add before publishing)
The following 10 files were not included and must be dropped in next to the HTML,
using these EXACT lowercase names (GitHub Pages is case-sensitive):

directions-strength.webp, faq.webp, step-hero.webp, stories-main.webp,
stories-side-01.webp, trust-nikita.webp, directions-crimea.webp,
directions-wear.webp, minatavr-hero.webp, stories-side-02.webp

See `images-manifest.txt` for which page uses what.

## Publish on GitHub Pages
1. Create a repository and upload the full contents of this folder to its root.
2. Add the 10 `.webp` images to the repo root (same folder as `index.html`).
3. Repo → Settings → Pages → Source: “Deploy from a branch”, branch `main`, folder `/ (root)`.
4. Open the published URL; the entry point is `index.html`.
