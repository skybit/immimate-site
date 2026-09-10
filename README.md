# ImmiMate public website

This directory contains the source for the public ImmiMate product, privacy, and support pages.

The site is intentionally static so it can be mirrored to the public GitHub Pages repository [`skybit/immimate-site`](https://github.com/skybit/immimate-site) without exposing the private application repository. The published URL is <https://skybit.github.io/immimate-site/>.

## Screenshots

The gallery contains ten current macOS Release-build captures from the official Immich Demo server (`https://demo.immich.app`). The capture contract and repeatable Appium workflow live in [`docs/qa/official-demo-marketing-screenshot-capture.md`](../docs/qa/official-demo-marketing-screenshot-capture.md); no credentials are committed.

## Local preview

From the repository root:

```bash
python3 -m http.server 4173 --directory website
```

Then open <http://127.0.0.1:4173/>.

## Publishing

Keep this directory as the source of truth. When the public pages change, mirror the contents of this directory to the `gh-pages` branch of `skybit/immimate-site`, preserving the repository's `.nojekyll` file.
