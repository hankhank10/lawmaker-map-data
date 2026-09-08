# Lawmaker map data

`Signyland.map` is the canonical game map for Lawmaker, in the Fantasy Map Generator format
(written by FMG v1.149.2). The map site loads it straight from this repository, so replacing the file
here publishes a new version of the world.

## Proposing changes

Open the map site with `?propose`, make your changes (rename, add, move or remove towns; rename
countries, provinces and rivers) and press **Submit on GitHub**. That opens a pre-filled issue here
labelled `proposal`. The maintainer reviews proposals on the site's `?review` page, applies the
accepted changes and uploads the new `Signyland.map` to this repository.

## Notes

- `.map` files are CRLF-delimited and must be stored byte-for-byte; `.gitattributes` marks them as
  not-text so git never normalises the line endings.
- The site, review tools and the delta format live in the (private) `lawmaker-map` repository.
