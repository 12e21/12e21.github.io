# Repository Guidelines

## Project Structure & Module Organization
- Site content lives in `_pages`, `_posts`, `_portfolio`, `_publications`, `_talks`, and `_teaching`; use the relevant folder before creating a new one. Posts follow `YYYY-MM-DD-title.md` with front matter.
- Shared layout and styling are in `_layouts`, `_includes`, `_sass`, and `assets`. Minified JS outputs to `assets/js/main.min.js`; source JS lives alongside it.
- Data-driven content (menus, profiles) sits in `_data`. Upload downloadable files to `files/`; images go to `images/`.
- Local copies of generated output appear in `_site` (git-ignored); do not edit that directory directly.

## Build, Test, and Development Commands
- `bundle install --path vendor/bundle` — install Ruby/Jekyll dependencies locally to `vendor/`.
- `bundle exec jekyll serve -l -H localhost` — run the site locally with live reload on `http://localhost:4000`.
- `npm install` — install JS tooling (uglify, onchange).
- `npm run build:js` — minify and bundle JS assets into `assets/js/main.min.js`.
- `npm run watch:js` — watch JS sources and rebuild the minified bundle on change.
- `docker compose up` — alternative local serve via the provided Docker setup.

## Coding Style & Naming Conventions
- Use 2-space indentation for YAML front matter and Liquid templates; keep Markdown wrapped at sensible line lengths for readability.
- Favor descriptive filenames; posts and collections should match existing patterns (`_posts/2023-10-05-title.md`).
- Keep front matter minimal and ordered (`title`, `date`, `layout`, `permalink`, tags/collections).
- JS edits should stay ES5-compatible unless you also adjust the build pipeline; keep changes in `assets/js/_main.js` and rebuild.

## Testing Guidelines
- No automated test suite is present; validate changes by running `bundle exec jekyll serve` and ensuring pages build without warnings.
- For JS changes, run `npm run build:js` and check the browser console for errors while serving locally.
- Before opening a PR, scan locally for broken links and missing assets; avoid committing `_site` or `vendor/` unless intentionally vendoring.

## Commit & Pull Request Guidelines
- Write concise, imperative commit messages (`Add talk page layout`, `Fix navbar spacing`). Group related changes per commit.
- Pull requests should summarize scope, list key changes, and note any screenshots for layout/visual updates.
- Link to related issues when applicable and describe how reviewers can reproduce the change locally (`bundle exec jekyll serve`, `docker compose up`).
- Ensure JS bundles are rebuilt if you touched source files; include the resulting `assets/js/main.min.js` in the PR when required.
