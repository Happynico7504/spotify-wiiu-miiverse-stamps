# Contributing Stamps

## What are stamps?

Stamps appear in the Miiverse post applet when sharing a track from Spotify Wii U. The Miiverse stamp system only supports black and white — all submitted images are automatically converted to 100×100 B&W by CI.

## Content rules

Pull requests that violate these rules will be closed without merging.

**Accepted:**
- Music-related imagery (instruments, notes, waveforms, album art interpretations)
- Abstract or geometric designs
- Spotify-related iconography (play/pause, shuffle, heart, etc.)
- Simple recognizable symbols and shapes

**Not accepted:**
- Explicit, sexual, or NSFW content of any kind
- Hate symbols, slurs, or content targeting any group
- Realistic depictions of real people (public figures or private individuals)
- Trademarked logos or copyrighted character art (brand wordmarks, Disney characters, game mascots, etc.)
- Low-effort submissions: solid colors, blank images, or images that produce no visible detail after B&W conversion
- Content that technically passes automated checks but is designed to evade review

## How to contribute

1. Add your image file to the repo root (PNG, JPG, BMP, GIF, or WebP — any size)
2. Add a row to [CREDITS.md](CREDITS.md) with your filename, a short description, and your GitHub username
3. Open a pull request targeting `main`

CI will automatically convert your image to 100×100 B&W and run a quality check. A maintainer will review the converted preview before merging.

## Quality check

CI fails if the converted B&W image is more than 98% a single color. This catches images that would appear invisible (all white) or as a solid block (all black) in the applet.

## Attribution

All stamps are released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). By submitting, you agree your contribution can be used, shared, and adapted under that license. Make sure you have the right to release any reference material you used.
