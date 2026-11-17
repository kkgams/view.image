# view.image

Image and Aseprite file Views for [GAMS](https://github.com/kkgams/gams). The local Project opens a file browser for your own PNG, JPEG, GIF, WebP, QOI or Aseprite files; no artwork is bundled.

| View | Source → deployed file | Screenshot | Original work |
| --- | --- | --- | --- |
| Image (`view-image`) | `src/view.image/views/view-image.js` → `views/view-image.js` | Not available | GAMS authors |
| Aseprite (`view-aseprite`) | `src/view.aseprite/views/view-aseprite.js` → `views/view-aseprite.js` | Not available | GAMS authors |

Both independently installable ZIPs include [Apache-2.0](LICENSE), [NOTICE](NOTICE) and [licensing scope](LICENSING.md).

## Development

Requires Make, Node.js, Python 3, curl, zip, unzip and tar. `make open` requires macOS Apple Silicon. Sources load directly; Host helpers and pinned released dependencies in `gams.json` are not bundled.

| Command | Purpose |
| --- | --- |
| `make open` | Open local Project in released Host; first launch needs network. |
| `make check` | Check JavaScript syntax. |
| `make package` | Build independent stable-name ZIPs and SHA256SUMS under `build.nosync/`. |
| `make serve-docs` | Preview pinned wiki; `DOCS_PORT=8081` overrides port 8080. |
| `make docs` | Build portable wiki in `build.nosync/site/`. |
| `make validate-docs` | Validate wiki links/content. |
| `make clean` | Remove all of `build.nosync/`, `tools/` and `gams_modules/`, without ownership markers; refuse tracked files or symlinks in deletion paths before deleting anything. |

Existing Host tools are never implicitly updated. Keep macOS security checks intact. GUI validation of file loading, canvas editing, timeline and export remains pending.
