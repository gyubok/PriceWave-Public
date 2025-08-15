# PriceWave (Private Source)

Private repo for PriceWave. A GitHub Action deploys `index.html`, `README.md`, and `LICENSE` to a separate **public** repo for GitHub Pages.

## Setup
1) Create a **public** repo, e.g., `pricewave-site`.
2) In this private repo: Settings → Secrets → Actions → **New secret**:
   - Name: `PUBLISH_TOKEN`
   - Value: fine‑grained PAT with **Contents: Read & Write** scoped only to the public repo.
3) Edit `.github/workflows/deploy.yml` — replace `<your-username>` and public repo name if different.

## Deploy
Push to `main`. The workflow copies files to the public repo and Pages deploys.

© 2025 — MIT
