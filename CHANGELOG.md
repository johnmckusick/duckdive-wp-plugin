# Release notes

Consumer-facing summary of each plugin release. (Full development history lives in the private source repository.)

## 2.6.9

- **Guard security check** — read-only endpoints MasterDoc calls once a day to report WordPress and plugin versions, administrators, application passwords, publishing totals, daily login counts, and recent content, plugin, and theme changes. Readable only by an Editor or above signed in with an application password; changes nothing on the site.

## 2.6.8

- **Leads grouped by visitor** — the DuckDive admin groups each visitor's phone views, clicks, and bookings into one journey.
- **ChatGPT Ads click IDs** — `campaign_id`, `ad_group_id`, `ad_id`, and `ad_account_id` are captured and attributed to ChatGPT Ads.
- **Lead export** — `/leads/export` returns leads for ROAS reporting, authenticated with the site's DuckDive API key.

## 2.6.7

- **ServiceTitan DNI timing fix** — waits for `dni('load')` before logging phone impressions so the swapped tracking number is captured instead of the static main line.

## 2.6.6

- **Phone impressions prefer visible DNI text** — captures the number shown on the page, not the stale `tel:` href.
- **Cross-page impression dedupe** — one impression per visitor + phone number per 30 minutes across page navigations.
- **Lead detail modal** — IP address now appears in Device & Browser.

## 2.6.5

- **Phone Number Display uses the bundled tracker** — when enabled, the plugin loads the local tracker script so impressions work even before the cloud tracker is updated on Render.

## 2.6.4

- **Phone Number Display is optional** — off by default; enable under DuckDive → Settings → Integrations for sites using DNI or manual-dial attribution.

## 2.6.3

- **Phone Number Display** — logs the visible DNI/`tel:` number when it appears on the page (including after ServiceTitan DNI swaps), so manual dialers can be attributed without a click.
- **Lead export enrichment** — `/leads/export` now includes visitor IP, user agent, and device/browser context for ROAS reporting.

## 2.5.9

- **Click to Call integration** — tel: link clicks are now a separate integration card from ServiceTitan Scheduling Pro.
- **ServiceTitan always on** — removed pilot hostname gate and auto-enable checkbox; works on any DuckDive-configured site.

## 2.5.8

- **ServiceTitan booking capture fix** — auto-loads the Scheduling Pro integration when the embed script is on the page; captures modal open (`BookingStarted`), contact info, and confirmed bookings via iframe postMessage and dataLayer hooks.

## 2.5.7

- **ServiceTitan integration logo** — added missing icon on the Settings integrations card.

## 2.5.6

- **Admin sidebar icon** — restored the SVG duck in the WP admin menu (PNG plugin icons remain on the Plugins list only).

## 2.5.5

- **New plugin logo** — updated icon in the WordPress Plugins list and DuckDive admin.
- **ServiceTitan Scheduling Pro** — plugin ready for booking and click-to-call capture (tracker updates are delivered via DuckDive cloud; no extra site config required).

## 2.5.4

- **Form tracking is always on** — Elementor, HubSpot, Go High Level, Contact Form 7, Gravity Forms, WPForms, and other supported builders are tracked automatically. No per-platform toggles required.
- **Fixed missing leads** — resolves an issue where saving plugin settings could turn off form integrations and stop leads from appearing in DuckDive while your CRM still received submissions.
- **Safer fallback** — if a platform integration is off, standard form capture still records the lead.

## 2.5.3

- Google Sheets sync skips gracefully when no spreadsheet URL is configured.

## 2.5.2

- Google Sheets lead export, refreshed admin branding, and settings improvements.

## 2.5.1

- Reorganized admin UI and scalable leads overview.

## 2.5.0

- Added support for Go High Level, Elementor Forms, Contact Form 7, Gravity Forms, WPForms, Ninja Forms, and Fluent Forms.

## 2.4.x

- HubSpot and Salesforce integration framework; automatic updates via this releases repository; improved signup and support messaging in settings.

## 2.3.x

- Improved HubSpot form capture and CSV export; client device context on leads; public update channel for WordPress sites.

## 2.2.x

- Performance improvements; HubSpot iframe and embed support; attribution injection for HubSpot forms.

## 2.1.x

- Advanced referrer mapping with DuckDive API key; rate limiting and security hardening.

## 2.0.0

- Universal automatic form capture; multi-touch attribution stored in WordPress.
