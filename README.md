# Kerala Light Intensity Analysis

A self-contained data report on the growth of nighttime light across Kerala,
India, **2012–2024** — statewide trend, district-by-district catch-up, decoupling
from physical built-up, population exposure, animated maps, and a Kollam district
spotlight.

The entire report is a single file, [`index.html`](index.html), with every chart,
GIF, and style embedded inline — no external assets, no build step.

## View it locally

Open `index.html` in any browser (double-click it, or `open index.html`).

## Publish on GitHub Pages

1. Create a new GitHub repository and push this folder to it:
   ```bash
   git remote add origin https://github.com/<you>/<repo>.git
   git branch -M main
   git push -u origin main
   ```
2. On GitHub: **Settings → Pages**.
3. Under **Build and deployment → Source**, choose **Deploy from a branch**.
4. Set **Branch** to `main` and folder to `/ (root)`, then **Save**.
5. After a minute your report is live at `https://<you>.github.io/<repo>/`.

The `.nojekyll` file tells GitHub Pages to serve the files as-is (skip Jekyll processing).

## Data sources

- **SVNL** — annual "NPP-VIIRS-like" nighttime-light reconstruction
  (figshare DOI [10.6084/m9.figshare.22262545](https://doi.org/10.6084/m9.figshare.22262545)).
  Radiance values are relative, not calibrated units.
- **GHSL** — EU Joint Research Centre Global Human Settlement Layer:
  GHS-BUILT-S (built-up surface) and GHS-POP (population), R2023A.
- **GADM** v4.1 — Kerala state, district, and sub-district boundaries.

Analysis and figures are reproducible from `scripts/kerala/` in the source project.
