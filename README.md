# harshiv-technologies

Generic developer website for Harshiv Technologies (Dhruvit Kachhiya). Hosts the **Developer Website**
and **Support URL** used in the App Store and Google Play Console listings for all apps.

Privacy Policy and Terms of Use pages are app-specific and live in each app's own repo (e.g.
`expense_tracker_web` for SpendGrid) &mdash; this repo intentionally does not duplicate them.

## Pages

- `index.html` &mdash; Developer profile with a list of apps and contact info. Use as the **Developer Website**.
- `support.html` &mdash; Contact details and FAQ. Use as the **Support URL**.

## Adding a new app

Add an entry to the `.app-list` section in both `index.html` and `support.html`:

```html
<div class="app-card">
  <h3>App Name</h3>
  <p>One-line description.</p>
  <div class="store-links">
    <a class="store-link" href="APP_STORE_URL">App Store</a>
    <a class="store-link" href="PLAY_STORE_URL">Google Play</a>
  </div>
</div>
```

## Tech

Plain HTML/CSS, no build step, no dependencies. Shared styling lives in `styles.css`.

## Deployment (GitHub Pages)

1. Push to the `main` branch.
2. In the repo on GitHub: **Settings → Pages → Source → Deploy from a branch**, branch `main`, folder `/ (root)`.
3. Site will be live at `https://kachhiyadhruvit1992.github.io/app-laboratory/`.
