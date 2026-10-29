# Forza Horizon 5 fan pages

Static multi-page fan site for three cars in **Forza Horizon 5**:

1. **1988 Chevrolet Monte Carlo Super Sport**
2. **2017 Acura NSX**
3. **2011 BMW X5 M Forza Edition**

## Tuned vs stock (do not mix)

| Page | Content |
|------|---------|
| `specs.html` | **TUNED** builds driven in FH5 (power, weight, times, grip, braking) |
| `desc.html` | **STOCK** in-game description summaries only |
| `upgrades.html` | Notes reading the published tunes + general Horizon advice |
| `index.html` | Home / the three cars |
| `board.html` | Static message board (form is non-functional) |

Tuned horsepower and times must never appear as stock figures, and stock summaries must never replace the tuned numbers on the specs page.

Footer note used on every page:

> Tuned figures are Forza Horizon 5 builds. Stock text is a short summary of the in-game description.

## Pages

- `index.html` — Welcome / the three cars
- `specs.html` — Tuned specs + comparison table
- `desc.html` — Stock descriptions
- `upgrades.html` — Upgrade notes
- `board.html` — Message board (static display)
- `styles.css` — Shared dark theme

## Run locally

No build step. Open any HTML file in a browser, or serve the folder:

```bash
cd forza-site
python3 -m http.server 8080
```

Then visit `http://127.0.0.1:8080/`.

## GitHub Pages

Push this folder as a repo (or as the `docs/` / root of a Pages branch). Enable GitHub Pages on the branch that contains these files. Paths are relative (`styles.css`, `index.html`, etc.) so they work from a project site root.

This repo is ready to push; nothing has been pushed yet.

## Source

Facts were taken from a local scrape of the original fan pages. Unicode ranges (0–60, ft·lb, N·m) are corrected from mojibake in the dump.
