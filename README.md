# Lawmaker map data

The game maps for Lawmaker. Every `<Name>.map` file in the root of this repository is shown on the map
site at `<site>/<name>` (lower-case), so `Signyland.map` is at `/signyland`. Replacing a file here
publishes a new version of that world; the site picks it up within a few minutes.

## Proposing changes

Open a map on the site with `?propose` (e.g. `/signyland?propose`), make your changes (rename, add,
move or remove towns; make a town a port; rename countries, provinces and rivers) and press
**Submit on GitHub**. That opens a pre-filled issue here labelled `proposal`. Each proposal is for one
map, named in the issue title.

## Notes

- `.map` files are CRLF-delimited and must be stored byte-for-byte; `.gitattributes` marks them as
  not-text so git never normalises the line endings.
- The site itself lives in the (private) `lawmaker-map` repository.
