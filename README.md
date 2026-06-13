# Spotify Wii U — Miiverse Stamps

Stamps that appear in the Miiverse post applet when posting from [Spotify Wii U](https://github.com/Happynico7504/spotify-wiiu).

## Using stamps in the app

Press **Stick L** while a track is playing to open the post applet. A pack picker will appear first — select a pack and press **A** to confirm. The selected pack is remembered for next time.

## Contributing stamps to this pack

Drop an image file into this repo and open a pull request. The CI pipeline will automatically convert it to the correct format (100×100, black and white) and sync it into the app.

**Supported formats:** PNG, JPG, BMP, GIF, WebP

Any size and color is fine — images are resized to 100×100 and converted to pure black and white automatically.

Please add a row to [CREDITS.md](CREDITS.md) with your filename, a short description, and your GitHub username.

## Creating your own stamp pack

1. Create a new public GitHub repo with your stamp images (any format, any name)
2. Add an entry to [`packs.json`](packs.json) in this repo pointing at your raw GitHub URL:
   ```json
   {
     "id": "your-pack-id",
     "name": "Your Pack Name",
     "description": "Short description",
     "base_url": "https://raw.githubusercontent.com/you/your-repo/main/"
   }
   ```
3. Open a pull request — once merged, your pack will appear in the in-app picker

Your images will be downloaded and converted automatically by the app when a user selects your pack. They do not need to be pre-converted.

## License

All stamps in this repo are released under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). See [CREDITS.md](CREDITS.md) for attribution.
