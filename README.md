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

## Airport announcements

The announcement panel uses the browser's Speech Synthesis API and an original four-note Web Audio chime. No cloud API key or external audio asset is needed. It is a simulation, not an official airport recording.

- Default sequence: **Cantonese → English → Mandarin**. Cantonese/English and single-language modes are also available.
- Choose a voice independently for each language, adjust volume/speed, preview the script, play and stop.
- Scripts use a snapshot of the current flight, destination, gate and status. Flight digits are spoken separately; Chinese gate numbers use normal number words.
- Missing voices are explicitly reported and skipped. Cantonese is never silently replaced by Mandarin. Use Refresh voices after enabling/installing system voices; online voices may need network access.
- Manual announcement types: current status, boarding soon, now boarding, final call, delayed and gate closed.
- Automatic announcements default to off. Opt in to status changes only, or status changes plus a five-/ten-minute interval. Automatic announcements always follow the displayed status, and do not play for no-status mode. Display language rotation never triggers speech.
- Press Stop to cancel the speech/chime queue and disable automatic announcements. The page stops queued announcements when closed. Background/locked devices may suspend speech or timers.
- The device must support Speech Synthesis for speech playback. Fullscreen does not affect the selected speech languages.

GA4 also receives `announcement_play` with only announcement status, language mode and whether the request was automatic. Flight/destination text is not added to analytics.

### Hong Kong terminal announcement style

Scripts use formal passenger-address language instead of conversational Cantonese, include bilingual airline names where available, and pronounce 24-hour estimated departure times as spoken hours/minutes. Optional codeshare reading is off by default. Default language gap is 1.5 seconds (adjustable to 0.8 or 2.5 seconds). Both Cantonese-English-Mandarin and Cantonese-Mandarin-English sequences are selectable.

These are original simulation templates, not an official transcript. Public references: [passenger recording of CX380 gate change announcement](https://www.youtube.com/watch?v=lA3BtoRVrHo) and [Cathay boarding instructions](https://flights.cathaypacific.com/zh_HK/travel-information/group-boarding.html). A single recording does not establish a universal language order. The synthesised chime is original; browser-native speech has no added terminal reverb and voice quality depends on the device.
