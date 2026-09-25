# vibezzzz-legal

The public pages for the **Vibezzzz** Android app, served by GitHub Pages:

| Page | URL |
|---|---|
| Landing page | https://amittal2001.github.io/vibezzzz-legal/ |
| Privacy policy | https://amittal2001.github.io/vibezzzz-legal/privacy/ |
| Affiliate disclosure | https://amittal2001.github.io/vibezzzz-legal/disclosure/ |

Those three URLs are submitted to Google Play, the App Store, TMDB, IGDB, and every affiliate network.
**Do not change a page's `permalink` once it has been submitted anywhere** — amending a filed
application is a multi-day round trip.

The app itself lives in the private `vibezzzz` repository.

## This repo contains prose only

Never add a GitHub Actions workflow or an Actions secret here. This repository is public, which means
anyone can fork it, every workflow file in it is world-readable, and its Actions logs would be
world-readable too. Every credential for this project belongs in the private `vibezzzz` repo, and
nowhere else.

## Editing

| File | |
|---|---|
| `index.md`, `privacy.md`, `disclosure.md` | the three pages — prose in Markdown, with the title, lede, and date in front matter |
| `_layouts/default.html` | the shared page shell: header, nav, footer |
| `assets/css/style.css` | the whole design, hand-written, light and dark |
| `assets/favicon.svg` | the mark, used as both favicon and header logo |
| `_config.yml` | site metadata, the `jekyll-seo-tag` plugin, and the default layout |

There is **no Jekyll theme**, so nothing here depends on an upstream project's markup or class names.
There is also no JavaScript, no web font, and no third-party request of any kind — a privacy page that
phoned home to a font CDN would undercut the thing it claims. Keep it that way.

Change the **"Last updated"** date (`updated:` in the front matter) in any page you edit — store
reviewers and the FTC both care that a published policy matches the shipped build.

Two `POST-LAUNCH` comments in `index.md` and `disclosure.md` mark the only edits that are waiting on
the Google Play release.
