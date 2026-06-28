# blit

Dirt-simple generator for blocky, mirror-symmetric avatar marks — deterministic from any name or email.

Every input hashes into a *variation of the base mark* (a 5×5 grid, drawn edge-to-edge in one blue). Same input always makes the same mark. Click a variation to promote it to the big view; download a crisp 1024px PNG.

## Run

No build step. Open `index.html`, or serve it:

```bash
python3 -m http.server 5633
```

## Knobs (top of the `<script>` / `<style>`)

- `BASE` — the base mark itself (left 3 columns of the 5×5, mirrored).
- `FLIP` — how far variations stray from the base mark (lower = closer).
- `--accent` — the one color marks are drawn in (`#4642d7`).
- `EXPORT_SIZE` — downloaded PNG resolution.

Wordmark, URL, and copy are plain text in the markup.
