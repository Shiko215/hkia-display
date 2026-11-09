# GATE 852

Free, unofficial Hong Kong airport gate display simulator.

**Website:** https://hkia.aurora-studio.org/

## Usage

Open `index.html` or `GATE_852.html` in a modern browser. Edit flights, choose a boarding status and language, then press F for fullscreen or Esc to return. Data stays in browser local storage. The upper-right clock uses Hong Kong time in 24-hour format; the estimated departure time is editable.

## GitHub Pages

Publish the repository root from `main`. `index.html` is the homepage. Keep `CNAME` for the custom domain. `GATE_852.html` is the equivalent standalone file; update both HTML files together. No build step is needed.

## Search and sharing

Canonical URL, bilingual visible product explanation and FAQ, WebSite/WebApplication/FAQPage JSON-LD, Open Graph and Twitter metadata, 1200×630 sharing image, robots.txt, sitemap.xml and a supplemental llms.txt are included. Structured data and llms.txt do not guarantee indexing, rankings, rich results or AI citations. Only the canonical homepage is listed in the sitemap.

## Analytics

Google Analytics 4 measurement ID: **G-RNN7G6DMYM**. The tag loads only on `hkia.aurora-studio.org`, not when opened from a local file or another hostname. It sends the default page view once and basic interaction events:

- `display_fullscreen_request`
- `display_language_select` (`language`)
- `display_rotation_toggle` (`enabled`)
- `display_status_select` (`boarding_status`)
- `display_preset_select` (`preset_index`)
- `display_flight_save`

Editable flight, destination and airline text is not included in custom analytics events. Initial page URLs omit query strings/fragments and the configured referrer includes only its origin. Google Signals and advertising personalisation signals are disabled. Visitors can disable analytics using the footer control; the preference is stored locally. GA4 enhanced-measurement settings are managed separately in Google Analytics.

To verify collection, visit the production website with analytics enabled and check the matching GA4 Realtime/DebugView report. Ad blockers, network policies and opt-out can prevent collection.

## Disclaimer

Unofficial simulation for entertainment. No live flight data. Not affiliated with, authorised or endorsed by Airport Authority Hong Kong or any airline. Rights in original designs and trademarks belong to their respective owners.
