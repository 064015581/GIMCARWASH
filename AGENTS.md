# AGENTS.md — GIM CAR WASH EXPRESS

## Project Overview
A single-page static HTML site (French) for a mobile car wash business. No build step, no backend, no dependencies — just `index.html` plus referenced (but currently missing) `assets/css/` and `assets/img/` directories.

## Running the App
```bash
docker compose -f docker-compose.base44.yml up -d
```
Serves `index.html` on port 3000 via a Python HTTP server with the repo bind-mounted read-only. Edits to `index.html` are reflected immediately on refresh (no rebuild needed).

## Notes
- The `assets/` directory referenced in `index.html` does not exist in the repo, so CSS and images currently 404. The page still renders with inline styles.
- No external credentials or secrets are needed.
