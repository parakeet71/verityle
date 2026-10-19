# Verityle

A static copy of Verityle from the [October 3, 2026 Internet Archive capture](http://web.archive.org/web/20261003212327/https://verityle.com/).

## How the game works

Choose eight images and submit your guess. Green means the image is in the correct position; yellow means it belongs in the combination but is in the wrong position. You have six guesses for each daily puzzle. Progress is saved in your browser.

## Provenance and rights

The original game files came from the archived site and were adapted for static hosting. The capture did not include a redistribution license; rights remain with their respective owners. See [`SOURCE.md`](SOURCE.md) for details.

## Run locally

Serve the `dist` directory over HTTP:

```sh
conda run -n main python -m http.server 8000 --directory dist
```

## Features added

- **AGAIN** button for starting another generated puzzle after the daily game.
