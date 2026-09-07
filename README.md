# Kibungan Pheno Hunt — Data Repo

Markdown record of truth for the **Kibungan** Filipino landrace pheno hunt,
ingested live from the shared #breeding Discord channel by
`monitor_breeding_notes.py`.

- `project.md` — project-level record
- `plants/<ID>.md` — one file per plant

This population uses **two** plant-ID prefixes, `PK` and `PL` (two seed
packs/batches of the same landrace); both route to this one project and repo,
so `plants/` holds both `PK##.md` and `PL##.md` files.

This repo is cloned and served by **breeding-data-api**
(`registry.json` → `github_repo: joeydouglas/kibungan-pheno-hunt`), which the
shared `breeding-frontend` renders. `.github/workflows/trigger-do-deploy.yml`
bumps the DigitalOcean app's CACHEBUST on every push so the API re-clones.

## Legacy static dashboard

The old generated HTML dashboard (`index.html`, `style.css`, `plants/*.html`
from `generate_dashboard.py`) moved to
**https://github.com/joeydouglas/kibungan-pheno-hunt-dashboard-legacy**
(NICK-701) so the data repo holds data only.
