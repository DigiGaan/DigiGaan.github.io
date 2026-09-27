# digigaan.github.io

Static site for the DigiGaan mobile app, served by GitHub Pages from the `main` branch root.

| Path | Purpose |
| --- | --- |
| `index.html` | Minimal landing page linking to the documents below |
| `privacy.html` | App privacy policy (store listings link here) |
| `delete-account.html` | Self-service account + data deletion (Play requires a web URL) |
| `app-ads.txt` | IAB Tech Lab authorized sellers declaration |
| `styles.css` | Shared stylesheet, light and dark |
| `.nojekyll` | Serve files as-is, skipping Jekyll processing |

## Before going live

1. Firebase Console -> Authentication -> Settings -> **Authorized domains** ->
   add `digigaan.github.io`, or Google Sign-In on the deletion page fails with
   `auth/unauthorized-domain`.
2. Confirm `USER_PATHS` in `delete-account.html` lists every Realtime Database
   tree keyed by uid. It currently deletes `users/$uid` only; any other
   top-level tree keyed by uid must be added or its data is orphaned.
3. Test the deletion page end to end with a throwaway Google account.
4. Set the Developer Website field in your Play Store / App Store listing to
   `https://digigaan.github.io` so ad networks can crawl `app-ads.txt`.
5. Add `https://digigaan.github.io/delete-account.html` to the Play Console
   Data Safety form as the account deletion URL.

Done already: Pages serves from `main` at `/`, `app-ads.txt` carries the live
AdMob and Meta Audience Network records, and the contact address throughout
`privacy.html` is `digigaan@gmail.com`.

## Verify

- https://digigaan.github.io/privacy.html
- https://digigaan.github.io/app-ads.txt (must return `text/plain`)
