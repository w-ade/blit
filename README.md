# blox

Dirt-simple generator for blocky, pixel-grid avatars — deterministic from any name or email.

Type a string and it hashes into a 5×5 mirrored identicon, drawn in a single accent color. Same input always makes the same mark. Download a crisp 1024px PNG.

## Run

No build step. Open `index.html`, or serve it:

```bash
python3 -m http.server 5633
```

## Knobs

- `--accent` — the one color avatars are drawn in (top of the `<style>` block).
- `EXPORT_SIZE` — downloaded PNG resolution (top of the `<script>` block).
- Wordmark, URL, and copy are plain text in the markup.

Fonts bundled in `fonts/`: [Geist Pixel](https://github.com/vercel/geistpixel-font) (Square / Grid / Line / Circle / Triangle).
