# GitHub Pages via Actions — Quick Start

This workflow publishes your static site (the `index.html` at the repository root) to GitHub Pages.

## Steps
1) Ensure your repo contains:
   - `index.html` at the root (plus README, LICENSE, .nojekyll if desired)
2) Add this file to your repo at `.github/workflows/pages.yml`
3) In **Settings → Pages → Build and deployment**, set **Source = GitHub Actions**.
4) Push to `main`. The workflow will run and publish your site.
5) The Pages URL appears on the repository home under the Environments section once deployed.

Notes:
- No separate branch is required with this method.
- If you prefer branch-based Pages instead, move `index.html` to the **gh-pages** branch root and set Source = Deploy from a branch (if available in your account).
