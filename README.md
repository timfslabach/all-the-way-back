# All the Way Back — the front door

One page. It carries the home-screen icon and the link preview that Apps Script can't, then sends you into the app.

## Links

- **Friends and your PT:** `https://timfslabach.github.io/all-the-way-back/` opens the view-only app.
- **You:** add your key after a `#`: `https://timfslabach.github.io/all-the-way-back/#me=YOUR_KEY`.
  The part after `#` never leaves your phone, so the key is not in this repo or on GitHub's servers.
  The page remembers it on that phone, so the plain link opens your owner view there too.
  To see exactly what friends see on your own phone, use `#view=friend`.

## Adding it to a home screen

Open the link with `&stay` on the end (yours: `…/#me=YOUR_KEY&stay`, friends: `…/#stay`) so it doesn't jump straight into the app.
Then Share → Add to Home Screen. From then on the icon opens straight into the app.

## If the app's web address ever changes

Change the one `href` on the `#go` link in `index.html`. That only happens if the Apps Script deployment is recreated instead of updated.

## Files

`index.html` the page · `icon-180.png` iPhone home screen · `icon-192/512.png` Android via `site.webmanifest` · `icon-32.png` browser tab · `og.png` the preview card in messages · `icon.svg`, `og.svg` sources for the images
