# openlych-site

Landing page for **OpenLych**: a local workbench for request flows.

Single page, no build step, no backend. Tailwind via CDN, light/dark with a
manual toggle (defaults to the system preference), brand colours pulled from
the app's own theme.

## Run

Just open `index.html`, or serve the folder:

```sh
python3 -m http.server 8000   # then open http://localhost:8000
```

## Structure

- `index.html`: the whole page (markup + Tailwind config + theme toggle)
- `assets/`: logo SVGs, favicon, app icon, screenshots

## Deploy

Served by GitHub Pages from `openlych/openlych.github.io` (`main`, root) at https://openlych.github.io/. Nothing to build.

## Keeping the page honest

The capabilities grid and the KDL sample on the page mirror what the app
actually ships: step types and function lists come from `src/model.rs` and
`src/kdlcfg.rs` in the OpenLych repo, and the sample snippets come from
`data/configs/`. Update this page in the same change when the engine gains or
renames a feature. The docs site (openlych-docs) is the deep reference; this
page links into it.
