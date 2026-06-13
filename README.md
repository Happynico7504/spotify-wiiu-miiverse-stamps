# Spotify Wii U — Miiverse Stamps

Stamps that appear in the Miiverse post applet when posting from [Spotify Wii U](https://github.com/Happynico7504/spotify-wiiu).

## Using stamps in the app

Press **Stick L** while a track is playing to open the post applet. A pack picker will appear first — select a pack and press **A** to confirm. The selected pack is remembered for next time.

## Contributing stamps to this pack

Drop an image file into this repo and open a pull request. The CI pipeline will automatically convert it to the correct format (100×100, black and white) and sync it into the app. See [CONTRIBUTING.md](CONTRIBUTING.md) for content rules and quality requirements.

**Supported formats:** PNG, JPG, BMP, GIF, WebP

Any size and color is fine — images are resized to 100×100 and converted to pure black and white automatically.

Please add a row to [CREDITS.md](CREDITS.md) with your filename, a short description, and your GitHub username.

## Creating your own stamp pack

1. Create a new public GitHub repo with your stamp images named `stamp1.png`, `stamp2.png`, … (100×100, black and white PNG)
2. Add an entry to [`packs.json`](packs.json) in this repo with the explicit filename list:
   ```json
   {
     "id": "your-pack-id",
     "name": "Your Pack Name",
     "description": "Short description",
     "base_url": "https://raw.githubusercontent.com/you/your-repo/main/",
     "stamps": ["stamp1.png", "stamp2.png", "stamp3.png"]
   }
   ```
3. Open a pull request — once merged, your pack will appear in the in-app picker

The `stamps` array is required. `raw.githubusercontent.com` does not support directory listing, so the app needs the explicit filenames to know what to download. Images must be pre-converted to 100×100 black and white PNG — unlike contributions to this repo, third-party packs are not auto-converted by CI.

## License

All stamps in this repo are released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). See [CREDITS.md](CREDITS.md) for attribution.
