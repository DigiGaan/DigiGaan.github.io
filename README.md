# digigaan.github.io

Static site for the DigiGaan mobile app, served by GitHub Pages from the `main` branch root.

| Path | Purpose |
| --- | --- |
| `index.html` | Minimal landing page linking to the documents below |
| `privacy.html` | App privacy policy (store listings link here) |
| `app-ads.txt` | IAB Tech Lab authorized sellers declaration |
| `styles.css` | Shared stylesheet, light and dark |
| `.nojekyll` | Serve files as-is, skipping Jekyll processing |

## Before going live

1. Replace `REPLACE_ME@example.com` in `privacy.html` (5 places) with a real contact address.
2. Replace `pub-0000000000000000` (AdMob publisher ID) and `000000000000000` (Meta Audience Network property ID) in `app-ads.txt`.
3. In the repo: Settings -> Pages -> Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
4. Set the Developer Website field in your Play Store / App Store listing to `https://digigaan.github.io` so ad networks can crawl `app-ads.txt`.

## Verify

- https://digigaan.github.io/privacy.html
- https://digigaan.github.io/app-ads.txt (must return `text/plain`)
