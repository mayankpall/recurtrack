# RecurTrack — public site

The marketing page, privacy policy and terms of use for the RecurTrack iOS app,
served by GitHub Pages at <https://mayankpall.github.io/recurtrack/>.

| File | What it is |
| --- | --- |
| `index.html` | The landing page. Self-contained: no build step, no dependencies, no external requests. |
| `privacy.html`, `terms.html` | The legal pages. |
| `_style.css` | Shared styling for the two legal pages only. |

Apple follows the privacy and terms links from the app's paywall during review,
so those two URLs must keep resolving. They are referenced in
`src/config/legal.ts` in the app repository.

The legal text's source of truth is the `docs/` folder of the app repository;
the copies here must be updated together with it. `_style.css` is presentation
only and is not mirrored back.

The landing page must not claim the app is on the App Store until it is.
