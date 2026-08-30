# Banner asset

`banner-source.svg` is the editable source for the profile banner. It uses DejaVu Sans so the export is reproducible on Linux.

Export `banner.png` from the repository root:

```bash
google-chrome --headless --disable-gpu --hide-scrollbars \
  --window-size=1584,396 \
  --screenshot=assets/banner.png \
  "file://$(realpath assets/banner-source.svg)"
```

The expected PNG dimensions are 1584 × 396 pixels.
