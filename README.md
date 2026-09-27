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

1. Set the Developer Website field in your Play Store / App Store listing to
   `https://digigaan.github.io` so ad networks can crawl `app-ads.txt`.
2. Confirm the app actually shows an EEA consent prompt before personalized
   ads, as section 5 of the privacy policy states.

Done already: Pages serves from `main` at `/`, `app-ads.txt` carries the live
AdMob and Meta Audience Network records, and the contact address throughout
`privacy.html` is `digigaan@gmail.com`.

## Verify

- https://digigaan.github.io/privacy.html
- https://digigaan.github.io/app-ads.txt (must return `text/plain`)
