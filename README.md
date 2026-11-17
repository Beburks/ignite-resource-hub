# Microsoft Ignite resource hub

A bright, responsive landing page for GitHub resources shared during a
Microsoft Ignite theater session.

## Edit or add a tile

Edit `site/index.html`. Each `.card` is a fully clickable resource tile.
Copy an existing card inside `.resource-grid`, update its URL and text, and
reuse a color class from `site/styles.css`. The grid expands automatically.

The adoption tile points to the documentation for AI adoption phases in the
Copilot usage dashboard, rather than a private dashboard.

## Preview

Run `python3 -m http.server 8000 --directory site` and open
`http://localhost:8000`. No dependencies or build step are needed.

## Publish

GitHub Pages is configured to use GitHub Actions. Changes to `site/` on `main`
deploy automatically through `.github/workflows/pages.yml`. You can also run
the workflow manually. Only `site/` is included in the published website.
