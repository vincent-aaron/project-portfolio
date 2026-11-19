# Ignition — Cars & Motorcycles, Curated

**Ignition** is a one-page showroom concept for supercars, performance cars, EVs, classics and motorcycles. It's a front-end portfolio piece built with plain HTML, CSS and vanilla JavaScript. There's no framework and no build step, just open `index.html`.

The UI borrows layout ideas from the big automotive websites, without copying any branding:
- full-screen hero sections with a slideshow and slide indicators
- a filterable model grid with spec chips
- side-by-side spec comparison with a sticky compare tray
- a test-drive booking flow

## Features

**Showroom**
- 24 vehicles (19 cars, 5 motorcycles) rendered from a single data array
- Category filter chips with counts (Supercar, Performance, Muscle, Electric & Hybrid, Classic, Motorcycle)
- Live search across make, model, engine and year, with a result count and an empty state that offers "Reset filters"
- Sort by featured, price, power, or 0–100 km/h time
- Detail dialog for every vehicle: large photo, description, full spec sheet, "Book a test drive" (pre-selects the car) and "Add to compare"

**Compare**
- Tick **Compare** on up to three vehicles. A floating tray shows your picks.
- Comparison table with animated bars and the best value highlighted for power, 0–100, top speed and price
- Shows a default hypercar vs. supercar vs. track-car match-up until you pick your own

**More sections**
- Hero slideshow with Ken Burns motion, progress-bar indicators and live captions; pauses on hover, on focus, and when the tab is hidden
- Animated stat counters, a brand marquee, and an Electric & Hybrid feature split with KPIs
- Motorcycles rail with scroll-snap and previous/next buttons
- Parallax quote band and a "Quickest to 100" leaderboard with animated bars (click a row to open that car)
- Test-drive form: inline validation, vehicles grouped by category, earliest date is tomorrow, friendly confirmation

**Accessibility & quality**
- Semantic landmarks, a skip link, labelled controls, `aria-pressed` on toggles, `aria-live` result counts
- Native `<dialog>` with Escape, backdrop click and focus return
- Respects `prefers-reduced-motion` (no autoplay, parallax or animations)
- Content is never left hidden: reveal styles only apply when JS runs, and a failsafe reveals everything after 2.5 s
- Responsive from 360 px phones (with a mobile menu) to wide desktops
- Lazy-loaded, dimensioned images (no layout shift); scroll effects run only while scrolling

## Tech Stack

| Area | Technology |
| --- | --- |
| Markup | HTML5 (`<dialog>`, landmarks, ARIA) |
| Styling | CSS custom properties, grid, `backdrop-filter`, scroll-snap |
| Scripting | Vanilla JavaScript, IntersectionObserver, `Intl.NumberFormat` |
| Fonts | Archivo (wide variable), Inter, JetBrains Mono (Google Fonts) |
| Images | Unsplash photos, saved locally and optimised (`images/`) |

## Project Structure

```
ignition-motors/
├── index.html    # Whole site: markup, styles, data and scripts
└── images/       # 31 optimised JPGs (hero, section banners, vehicle cards)
```

To add or edit a vehicle, change the `V` array at the top of the `<script>` in `index.html`. Cards, filters, counts, the compare table, the leaderboard and the booking dropdown all update automatically.

## Running Locally

Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
# or
python -m http.server 8000
```

## Deploying

The site is fully static. For GitHub Pages: **Settings → Pages → Deploy from a branch → `main` / root**.

## Notes

- Ignition is a fictional showroom built as a portfolio concept. Prices are placeholders, and the booking form sends nothing.
- Specs are approximate published figures. The Tesla Roadster figures are the manufacturer's claims for an unreleased model, so it's left out of the leaderboard.
- Photography is from [Unsplash](https://unsplash.com). Vehicle names and trademarks belong to their respective owners.

## Author

**Vincent Aaron** — [github.com/vincent-aaron](https://github.com/vincent-aaron)
