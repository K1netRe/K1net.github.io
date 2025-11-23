# K1net Blog (Hexo)

This repository uses Hexo to generate a static site. Basic commands:

- `npm run build` — generate static files into `public/`.
- `npm run clean` — remove generated files.
- `npm run deploy` — deploy using local `hexo deploy` (if configured).
- `npm run server` — run local dev server.

Deployment (recommended):
- This repo includes a GitHub Actions workflow `.github/workflows/deploy.yml` that builds the site and publishes `public/` to the `gh-pages` branch using the automatically provided `GITHUB_TOKEN` (no personal token required).
- If you prefer to continue using `hexo deploy` locally, do NOT store personal access tokens in `_config.yml`. Use SSH deploy or environment variables / CI secrets instead.

Security note:
- You previously exposed a GitHub PAT in `_config.yml`. Ensure you revoke it on GitHub (Settings → Developer settings → Personal access tokens) and rotate any credentials used elsewhere.
