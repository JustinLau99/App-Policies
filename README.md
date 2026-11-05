# App-Policies

Public HTML privacy policies and disclaimers for app store listings.

Hosted with [GitHub Pages](https://pages.github.com/) from this repository.

## Layout

```text
App-Policies/
└── docs/
    ├── index.html
    ├── pricescan/
    │   ├── privacy.html
    │   └── disclaimer.html
    └── audiotext/          # add when ready
        ├── privacy.html
        └── disclaimer.html
```

- **`docs/`** — all published HTML lives here (keeps the repo root clean for README, license, etc.).
- **One folder per app** — use a short slug (`pricescan`, `audiotext`, …).
- **`privacy.html`** — data collection, third parties, contact.
- **`disclaimer.html`** — legal disclaimers separate from privacy (e.g. not financial advice).

## Published URLs

Enable Pages from the **`/docs`** folder (see below). URLs look like:

| App       | Privacy | Disclaimer |
|-----------|---------|------------|
| PriceScan | `https://justinlau99.github.io/App-Policies/pricescan/privacy.html` | `https://justinlau99.github.io/App-Policies/pricescan/disclaimer.html` |

Index: `https://justinlau99.github.io/App-Policies/`

Use the **privacy** URL in Google Play and App Store Connect. Link the **disclaimer** from the app or store listing if needed.

## Enable GitHub Pages

1. Push this repo to `JustinLau99/App-Policies`.
2. On GitHub: **Settings → Pages**.
3. **Build and deployment → Source:** Deploy from a branch.
4. **Branch:** `main`, folder **`/docs`**.
5. Save. The site may take a few minutes to go live.

## Adding another app

1. Create `docs/<app-slug>/privacy.html` and `docs/<app-slug>/disclaimer.html` (omit disclaimer if not needed).
2. Add an entry in `docs/index.html` with links to both files.
3. Default contact: `justinlau99dev@gmail.com` unless the app uses a different address.

## Source of truth

Edit policies **here**. App repos should link to these public URLs, not maintain a second copy.
