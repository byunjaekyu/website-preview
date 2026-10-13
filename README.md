# BYUN JAEKYU — Artwork data starter

This is a **prototype**, not a full replacement for the existing website. Back up the existing `index.html` before replacing it. The prototype currently includes one work; migrate the other existing works and the Research/About/CV content before publishing.

1. Add a folder under `works/` for each new artwork.
2. Add `info.md` with YAML metadata between `---` lines and description below.
3. Place images inside that work's folder; use relative filenames in `cover` and `images.file`. To reuse images already in the repository's root `images/` folder, use `images/name.jpg`.
4. Push to GitHub `main`. GitHub Actions builds `works.json` and commits it, which GitHub Pages can serve.
5. For local preview, install `pyyaml`, run `python scripts/build.py`, then `python -m http.server 8000`.

For a work with `cover: main.jpg`, the file must exist at `works/<slug>/main.jpg`.

Before publishing, verify GitHub Actions has permission to write repository contents. Ensure GitHub Pages is set to deploy from the `main` branch. The prototype's CV, Research and About are placeholders and must not replace existing public content without migration.
