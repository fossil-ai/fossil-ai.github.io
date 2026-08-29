# fossil-ai.github.io

Personal site for **Faisal Mohammad** — Senior Applied Research Engineer.
Hand-built, single-file static site. No frameworks, no build step: just `index.html`.
Served by GitHub Pages at **https://fossil-ai.github.io**.

```
.
├── index.html   ← the whole site (HTML + CSS + JS). Edit this.
├── favicon.svg  ← the "F" tab icon
├── .nojekyll    ← makes GitHub Pages serve files as-is (no Jekyll build)
├── assets/      ← put cv.pdf, profile.jpg, og-image.png here
└── README.md
```

> This repo previously hosted a Beautiful Jekyll site. That version is preserved in git
> history and tagged **`pre-2026-redesign`** — recover it any time with
> `git checkout pre-2026-redesign`.

## Editing

Open `index.html` and search for `EDIT:` — every spot to personalize is marked. Current
placeholders to fill in:

- **Employment dates** + a quantified win or two (Experience section).
- **LinkedIn URL** (Contact section) — recruiters look for it.
- **Résumé** — drop your PDF at `assets/cv.pdf` (the Résumé buttons point there).
- **Coursework** — real graduate courses, or delete that block.
- Optional **headshot** — add `assets/profile.jpg` and swap the `.avatar` div (see the note in the CSS).

Colors/type live in the `DESIGN TOKENS` block at the top of the `<style>` — change `--accent`
to restyle everything.

## Preview locally

```bash
python3 -m http.server 8000    # then open http://localhost:8000
```

## Deploy (already a GitHub Pages repo)

Pages is already configured for this repo, so publishing is just a push:

```bash
git add -A
git commit -m "Redesign: static single-page site"
git push origin master
```

Live within ~1 minute at **https://fossil-ai.github.io**. If Pages isn't enabled, set it under
**Settings → Pages → Deploy from a branch → `master` / root**.
