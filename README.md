# UAE Activity Pulse

UAE Activity Pulse is an independent public-data project that turns recurring UAE government datasets into concise signals about real-world activity.

The goal is simple:

> Preserve public data over time, detect what changed, and publish useful observations.

## Current coverage

### Dubai Commercial Leasing Pulse

A weekly view of newly registered physical commercial leases in Dubai, including:

- total new physical commercial leases
- office, shop, warehouse and other property types
- most active areas
- week-on-week movements
- persistent activity patterns
- selected residential occupancy signals

Virtual units and multi-property registrations are excluded from the core commercial analysis.

## Other signals being explored

- Construction activity
- Residential occupancy / mover signals
- Other Emirates
- Additional UAE public datasets

## Methodology

The project prioritizes:

- transparent filtering
- preserving recurring snapshots
- separating observed movement from long-term trends
- documenting data limitations
- using official public sources wherever possible

Full methodology is published on the website.

## Data sources

Current reports use publicly available data from the Dubai Land Department.

UAE Activity Pulse is an independent project and is not affiliated with Dubai Land Department or any UAE government entity.

## Website

The website is a lightweight static site designed for Cloudflare Pages.

Main files:

- `public/index.html`
- `public/reports/`
- `public/archive/`
- `public/methodology/`
- `public/about/`

## Deployment

The site can be deployed directly from this GitHub repository using Cloudflare Pages.

Build command: none

Output directory:

```text
public