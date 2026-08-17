# Backflow Log public site

Static, dependency-free marketing, support, and privacy pages for Backflow Log,
following the Good Little Apps site conventions.

## Production URLs

- Marketing: `https://good-little-apps.github.io/backflow/`
- Support: `https://good-little-apps.github.io/backflow/support.html`
- Privacy: `https://good-little-apps.github.io/backflow/privacy.html`

## Zero-cost GitHub Pages deployment

1. Create a **public** GitHub repository named `backflow` under the
   `good-little-apps` account.
2. Place the contents of this folder at the repository root.
3. In **Settings → Pages**, choose **Deploy from a branch**, branch `main`,
   folder `/ (root)`.
4. Wait for the Pages deployment, then open every production URL above in a
   private browser window.
5. Do not configure a custom domain. The `github.io` address is free and can
   be used as the App Store support and privacy URLs.

No build system, package manager, server, database, analytics, cookie
banner, or paid service is required. GitHub Pages hosts the files directly
over HTTPS.

## Preflight

- Check internal links from all three pages.
- Confirm the privacy page matches `../PRIVACY.md` and the shipping binary.
  As of build 11 that means: no purchases, but the app *does* schedule local
  notifications (opt-in, no push server) and *does* export and restore a
  backup file. Both are described on the privacy and support pages; revisit
  them whenever a release changes what leaves the device.
- Confirm the public email can send and receive.
- Test at 320 CSS pixels wide, with keyboard-only navigation and increased
  browser text size.
- Run an HTML validator if available; GitHub Pages should publish the files
  unchanged.
- Add the App Store link to `index.html` only after Apple provides the
  final public URL.
