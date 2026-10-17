# fossil-ai.github.io

Personal site for **Faisal Mohammad**, served by GitHub Pages at **https://fossil-ai.github.io**.

One plain `index.html`: no frameworks, no JavaScript, no build step.

```
.
├── index.html   ← the whole site. Edit this.
├── favicon.svg
├── .nojekyll    ← makes GitHub Pages serve files as-is (no Jekyll build)
└── assets/      ← optional profile.jpg, cv.pdf
```

> The older Beautiful Jekyll site is tagged **`pre-2026-redesign`** (`git checkout pre-2026-redesign`).

## Editing

- **New paper:** copy an `<li>` in the Publications list. Put your own name in `<b>`.
- **Headshot:** add `assets/profile.jpg` and it fills the photo panel next to the intro automatically.
- **CV / Scholar / LinkedIn:** add another `<a>` to the `.links` line in the header.
- Bump the "Last updated" footer when you change something.

## Preview locally

```bash
python3 -m http.server 8000    # then open http://localhost:8000
```

## Deploy

```bash
git add -A && git commit -m "Update site" && git push origin master
```
