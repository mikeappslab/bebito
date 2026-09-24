# Bebito legal site (GitHub Pages)

Plain static pages — no build step, no JavaScript.

Files: `index.html`, folder pages (`privacy/`, `terms/`, `disclaimer/`,
`acknowledgements/`, `support/`), thin `*.html` redirects for old URLs,
`style.css`, logo files and `.nojekyll` (tells GitHub Pages to serve the
files as-is).

## Option A — publish from this repo

1. Push this repository to GitHub.
2. GitHub → **Settings → Pages**.
3. Source: **Deploy from a branch**, branch `main`, folder **`/docs`**. Save.
4. After a minute the site is live at
   `https://<username>.github.io/<repository>/`.

## Option B — a separate repo just for the site

1. Create a repo, e.g. `bebito-legal`.
2. Copy the **contents** of this `docs/` folder into the repo root.
3. Settings → Pages → Deploy from a branch, branch `main`, folder **`/ (root)`**.

## Links for App Store Connect

- Privacy Policy URL: `https://<user>.github.io/<repo>/privacy/`
- Terms of Use (EULA) URL: `https://<user>.github.io/<repo>/terms/`
- Support URL: `https://<user>.github.io/<repo>/support/`

Old `*.html` URLs still redirect to these folder paths.

## Keeping the text in sync

The wording matches the in-app legal pages (English strings under `legal.*`
in `src/lib/i18n/locales/en.json`). If you change one, change the other and
update the "Last updated" date at the bottom of the page.
