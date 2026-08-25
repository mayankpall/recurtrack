# RecurTrack — public site

The marketing page, privacy policy and terms of use for the RecurTrack iOS app,
served by GitHub Pages at <https://recurtrack.mayankpal.co.in>.

The custom domain is a `CNAME` DNS record pointing `recurtrack` at
`mayankpall.github.io`, plus the `CNAME` file GitHub writes into this repo. Do
not delete that file — removing it drops the domain and breaks the URLs Apple
has on file. The old `mayankpall.github.io/recurtrack/` URLs still 301 here.

| File | What it is |
| --- | --- |
| `index.html` | The landing page. Self-contained: no build step, no dependencies, no external requests. |
| `privacy.html`, `terms.html` | The legal pages. |
| `_style.css` | Shared styling for the two legal pages only. |

Apple follows the privacy and terms links from the app's paywall during review,
so those two URLs must keep resolving. They are referenced in
`src/config/legal.ts` in the app repository, which is the canonical spelling of
them — App Store Connect has the same two on file.

The legal text's source of truth is the `docs/` folder of the app repository;
the copies here must be updated together with it. `_style.css` is presentation
only and is not mirrored back.

The landing page must not claim the app is on the App Store until it is.
