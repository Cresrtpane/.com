# Crestpane website

Static multi-page site (HTML, CSS, JavaScript). No build step is needed to host it.

## Deploy on GitHub Pages
1. In the `Crestpane.github.io` repository, delete the old files, then upload everything from this folder (keep `.nojekyll`).
2. Settings, Pages, deploy from the `main` branch root.
3. Live at https://crestpane.github.io/

## Edit content
Content lives in `_generator/data.py` (services, projects, blog articles, FAQ, pricing and the calculator rules).
Set the domain in `SITE_URL` there, then run `python3 build.py` inside `_generator` (run it from a folder next to `site/`), which regenerates all pages, sitemap and robots.txt.

## Forms
There is no server. Forms prepare a message that visitors send via Telegram or email themselves. To receive submissions directly, connect a form service and replace the handler in `assets/main.js`.
