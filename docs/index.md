---
title: view.image
status: reference
---

# view.image

The local Project opens a file browser. Select your own Project-local PNG, JPEG, GIF, WebP, QOI or Aseprite file to open the local image/aseprite View. No artwork is bundled.

The local Project registers canonical View entries directly from `src/` and published dependencies pinned in `gams.json`. Host-owned `/core`, `/util`, `/widgets` APIs and theme styling are not bundled.

Run `make open` on macOS Apple Silicon to launch the real Host. Run `npm test` for repository checks. Preview docs with `make serve-docs DOCS_PORT=8081`, validate with `make validate-docs`, and build a portable site with `make docs`. GitHub Pages runs that build on every push to `release`. Unit tag-release policies are unchanged.
