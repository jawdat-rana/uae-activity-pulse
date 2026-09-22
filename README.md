# UAE Activity Pulse — V1

A dependency-free static website for publishing recurring UAE public-data reports.

## Structure

- `public/index.html` — homepage
- `public/reports/` — full weekly reports
- `public/archive/` — report archive
- `public/methodology/` — methodology and limitations
- `public/about/` — project positioning
- `public/assets/styles.css` — site styling
- `public/_headers` — basic security headers for Cloudflare Pages

## Recommended Cloudflare Pages deployment

Because this project is intended to receive weekly automated updates, use **Git integration from the start** rather than Cloudflare Pages Direct Upload.

1. Create a GitHub repository, e.g. `uae-activity-pulse`.
2. Copy the contents of this folder into the repository.
3. In Cloudflare: **Workers & Pages → Create → Pages → Connect to Git**.
4. Select the repository.
5. Build command: leave blank.
6. Build output directory: `public`
7. Deploy.

Cloudflare will give you a `*.pages.dev` URL.

### Custom domain later

A custom domain can be attached later from the Pages project's **Custom domains** section. The existing `pages.dev` URL can remain active or be redirected later.

## Weekly publishing workflow

V1 is intentionally static.

For each new report:
1. Add a new HTML page under `public/reports/`.
2. Add it to `public/archive/index.html`.
3. Update the homepage latest numbers / observations.
4. Commit and push.
5. Cloudflare Pages redeploys automatically.

The next automation step can generate these pages directly from the weekly analysis output.

## Design direction

- Editorial/data-publication rather than SaaS dashboard
- Broad brand: can cover multiple Emirates and multiple domains
- Current live signal: Dubai Commercial Leasing
- Construction Activity: experimental
- Residential Occupancy: exploratory
- No external fonts, JavaScript frameworks, trackers or paid dependencies

## Before public launch

Optional additions:
- Add an email/contact destination if desired.
- Add analytics only if useful; Cloudflare Web Analytics is enough for V1.
- Add a custom domain later.
