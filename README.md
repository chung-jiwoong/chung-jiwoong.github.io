# chung-jiwoong.github.io

Source for my personal academic website, built with [Quarto](https://quarto.org).

| Path | What it is |
| --- | --- |
| `index.qmd` | Home page |
| `cv.qmd` | CV — renders to both HTML and PDF (via Typst) |
| `research.qmd` | Papers |
| `teaching.qmd` | Courses |
| `_quarto.yml` | Site config (nav, theme, metadata) |
| `styles.css` | Custom CSS |
| `docs/` | **Generated output — do not edit by hand.** GitHub Pages serves this folder |

## Editing

Edit the `.qmd` files, then:

```sh
quarto preview     # live preview while editing
quarto render      # write output to docs/
```

Commit the source changes. Pushing to `main` triggers
[`.github/workflows/publish.yml`](.github/workflows/publish.yml), which
re-renders the site and commits `docs/` automatically — so the published site
cannot drift behind the sources.

## Pages configuration

Settings → Pages → Deploy from a branch → `main` / `docs`.
