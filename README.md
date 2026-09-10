# Backflow Log public site

Static, dependency-free marketing, support, and privacy pages for Backflow Log,
following the Good Little Apps site conventions.

## Production URLs

- Marketing: `https://good-little-apps.github.io/backflow/`
- Support: `https://good-little-apps.github.io/backflow/support.html`
- Privacy: `https://good-little-apps.github.io/backflow/privacy.html`

## Existing GitHub Pages deployment

The public site repository is `https://github.com/good-little-apps/backflow`.
It is separate from the app source repository. Pages publishes `main` at `/`.

1. Compare this folder with the latest public repository before editing.
2. Copy only the site files to the public repository root.
3. Commit and push the changes to that repository's `main` branch.
4. Wait for the Pages deployment and verify all three production URLs.

No build system, package manager, server, database, analytics, cookie
banner, or paid service is required. GitHub Pages hosts the files directly
over HTTPS.

## Preflight

- Check internal links from all three pages.
- Confirm the privacy page matches `../PRIVACY.md` and the shipping binary.
  The app currently has no purchases, but the app *does* schedule local
  notifications (opt-in, no push server) and *does* export and restore a
  backup file. Both are described on the privacy and support pages; revisit
  them whenever a release changes what leaves the device.
- Confirm the public email can send and receive.
- Test at 320 CSS pixels wide, with keyboard-only navigation and increased
  browser text size.
- Run an HTML validator if available; GitHub Pages should publish the files
  unchanged.
- Keep the download link pointed at the live App Store listing:
  `https://apps.apple.com/us/app/backflow-log/id6799603346`.
