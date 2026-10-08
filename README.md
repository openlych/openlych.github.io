# openlych-site

Static showcase site for **OpenLych** — a local web-testing workbench.

Single page, no build step, no backend. Tailwind via CDN, light/dark with a
manual toggle (defaults to the system preference), brand colours pulled from
the app's own theme.

## Run

Just open `index.html`, or serve the folder:

```sh
python3 -m http.server 8000   # then open http://localhost:8000
```

## Structure

- `index.html` — the whole page (markup + Tailwind config + theme toggle)
- `assets/` — logo SVGs, favicon, app icon

## TODO before publishing

- Swap the `github.com/your/openlych` links for the real repo + releases URLs.

## Deploy

Any static host (GitHub Pages, Netlify, a plain web server). Nothing to build.
