# Williamstown Special Nights

Every weeknight special across Williamstown, Newport & Spotswood — steak nights, parmas,
trivia, roasts and kids-eat-free deals — mapped, rated and ranked.

Single self-contained `index.html`. No build step, no dependencies beyond Google Fonts
and a CDN-hosted Leaflet (used on the Map tab).

## GitHub Pages setup
1. Push `index.html` and `.nojekyll` to the repo root on `main` (or `master`).
2. Repo → **Settings → Pages**.
3. Source: **Deploy from a branch**.
4. Branch: `main`, folder: **/ (root)**.
5. Save. Pages builds in ~1 minute and gives you a `https://<username>.github.io/<repo>/` URL.

The `.nojekyll` file tells GitHub Pages to skip Jekyll processing and serve the file as-is —
needed because this isn't a Jekyll site and Jekyll would otherwise ignore files/folders
starting with an underscore and try to process Liquid syntax.

## Updating
All venue data, specials, ratings and scores live in the `V` array inside the `<script>`
block of `index.html`. Edit a price, score, or special there, commit, and push — Pages
redeploys automatically on every push to the Pages branch.

Data last checked: 27 Jun 2026.
