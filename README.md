# App-Policies

Public HTML privacy policies (and disclaimers where needed) for app store listings.

Hosted with [GitHub Pages](https://pages.github.com/) from this repository.

## Layout

```text
App-Policies/
├── index.html              # Directory of all apps
├── pricescan/
│   └── privacy.html        # PriceScan — privacy + financial disclaimer
└── <future-app>/
    └── privacy.html
```

One folder per app. Keep each app’s policy in a single `privacy.html` unless you later split terms/disclaimer into separate pages.

## Published URLs

After Pages is enabled (see below), links look like:

| App       | Policy URL |
|-----------|------------|
| PriceScan | `https://justinlau99.github.io/App-Policies/pricescan/privacy.html` |

Use the **PriceScan** row as the privacy policy URL in Google Play and App Store Connect.

## Enable GitHub Pages

1. Push this repo to `JustinLau99/App-Policies`.
2. On GitHub: **Settings → Pages**.
3. **Build and deployment → Source:** Deploy from a branch.
4. **Branch:** `main`, folder **`/ (root)`**.
5. Save. The site may take a few minutes to go live.

## Before you publish

1. Push to GitHub and enable Pages (see above).
2. When you add another app, create `<app-slug>/privacy.html` and add a row in `index.html`.
3. Use the same contact email (`justinlau99dev@gmail.com`) in new policies unless an app needs a different address.

## Source of truth

Edit policies **here**, not only in individual app repos. The copy under `pricescan/docs/` in the PriceScan app repo can stay as a draft or be removed to avoid drift—**App-Policies** is the canonical public version.

## Adding another app

1. Create `your-app-slug/privacy.html` (self-contained HTML, same pattern as PriceScan).
2. Add a list item in `index.html` linking to `your-app-slug/privacy.html`.
3. Commit, push, and use the new GitHub Pages URL in the store listing.
