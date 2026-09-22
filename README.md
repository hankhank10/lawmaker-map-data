# Lawmaker map data

The game maps for Lawmaker. Every `<name>.map` file in the `maps/` folder of this repository is shown on the map
site at `<site>/<name>` (lower-case), so `maps/signyland.map` is at `/signyland`. Replacing a file here
publishes a new version of that world; the site shows it on the next page load.

## Proposing changes

Open a map on the site with `?propose` (e.g. `/signyland?propose`), make your changes (rename, add,
move or remove towns; make a town a port; rename countries, provinces and rivers) and press
**Submit on GitHub**. That opens a pre-filled issue here labelled `proposal`. Each proposal is for one
map, named in the issue title.

## Proposing a new map

Open the site's landing page and choose **Propose a new map** (`/propose-new-map`): generate a continent,
shape its land, draw countries, provinces, rivers and towns, and submit it. The game files it here as a
**pull request** labelled `new-map` that adds `maps/<name>.map` (and `maps/<name>.png`, the landing page's
picture of it). Every country in a proposed map is named "Unknownia"; countries are named through change
proposals once the map is live. Merging the pull request publishes the map.

## Notes

- `.map` files are CRLF-delimited and must be stored byte-for-byte; `.gitattributes` marks them as
  not-text so git never normalises the line endings.
- `maps/<name>.png` next to a map is optional: the site shows it on the landing page when present.
- The labels `proposal` (change proposals, issues) and `new-map` (new maps, pull requests) must exist here.
- The site itself lives in the (private) `lawmaker-map` repository.
