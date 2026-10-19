# Verityle

A static copy of the Verityle game from the [October 3, 2026 Internet Archive capture](http://web.archive.org/web/20261003212327/https://verityle.com/). The archived game bundle, styling, images, and sounds are included; no build or package installation is needed.

Choose eight images and submit a guess. Green marks an image in the right position; yellow marks an image in the wrong position. There are six guesses per daily puzzle. You can also use the 1–4 keys, Backspace, and Enter. The puzzle uses your browser's local date, and progress is saved in local storage.

## Run locally

Serve the `dist` directory over HTTP, for example with the `main` Conda environment:

```sh
conda run -n main python -m http.server 8000 --directory dist
```

Then visit `http://localhost:8000/`.

## Deploy to GitHub Pages

1. Push this repository to GitHub.
2. In the repository settings, under **Pages**, set the build and deployment source to **GitHub Actions**.
3. Push to the repository's default branch, or run the **Deploy to GitHub Pages** workflow from the Actions tab on that branch.

The workflow publishes `dist` directly. Asset paths are relative, so the game also works at a project URL such as `https://username.github.io/repository/`.

The bundled code has been adjusted to use local, relative asset paths, omit Vercel analytics, and put the current page URL in copied results. Wayback Machine scripts and advertising have been omitted from the HTML.

## Provenance and rights

The capture did not include a redistribution license. Before publishing this copy, confirm that you own the original material or otherwise have permission to republish its code, images, and sounds. See `SOURCE.md` for the capture URL, packaging changes, and file hashes.
