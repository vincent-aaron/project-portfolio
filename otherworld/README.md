# Novel Plus — Otherworld Books

**Otherworld** is a single-page storefront concept for an independent light novel shop specialising in isekai, fantasy and slice-of-life titles. It is a front-end design project that focuses on editorial typography, photography and smooth, accessible motion — built with plain HTML, CSS and vanilla JavaScript, no frameworks or build step.

## Features

**Sections**
- **Hero** with a full-bleed parallax photo, word-by-word headline reveal, catalog search and animated stats counters
- **Genre marquee** that scrolls continuously and pauses on hover
- **New arrivals**: six featured light novels with cover art, genre tags, authors and prices
- **Browse by genre**: six photo cards (Isekai, High Fantasy, Slice of Life, Villainess, Dungeon & Kingdom Building, Reverse Isekai)
- **Quote band**, **Top sellers** ranking with trend indicators, **About** story, and a **Newsletter** sign-up
- Sticky navigation with scroll-spy highlighting of the current section

**Interactions**
- **Catalog search** filters the book cards by title, author or genre tag, shows a match count, and has a "Show all" reset
- Scroll-triggered fade, image wipe and word-mask reveals (IntersectionObserver)
- Scroll-driven parallax layers, recalculated only while scrolling or resizing
- Magnetic buttons and 3D tilt on book and genre cards (mouse/trackpad only)
- Newsletter form with inline confirmation (front-end demo, no emails are sent)

**Accessibility & resilience**
- Honours `prefers-reduced-motion` (animations, parallax and counters are switched off)
- Content is never left hidden: reveal styles apply only when JavaScript runs, errors fall back to showing everything, and a 2-second failsafe reveals anything still hidden
- Visible keyboard focus styles, labelled form fields, descriptive alt text on covers
- Responsive layout from mobile to wide desktop
- Below-the-fold images are lazy-loaded

## Tech Stack

| Area | Technology |
| --- | --- |
| Markup | HTML5 |
| Styling | CSS (custom properties, grid, `clip-path`) |
| Scripting | Vanilla JavaScript (ES5-compatible) |
| Fonts | Fraunces, Inter, IBM Plex Mono (Google Fonts) |

## Project Structure

```
novel-plus/
├── index.html      # The whole site: markup, styles and scripts
└── images/         # Optimised JPGs used by the page
    ├── hero-opt.jpg, arrivals-banner-opt.jpg, quote-band-opt.jpg, ...
    ├── book-*-cover-opt.jpg     # Book covers
    └── genre-*-opt.jpg          # Genre card photos
```

## Running Locally

Open `index.html` in a browser, or serve the folder:

```bash
npx serve .
# or
python -m http.server 8000
```

## Deploying

The site is fully static. To publish with GitHub Pages: **Settings → Pages → Deploy from a branch → `main` / root**.

## Notes

- This is a portfolio/demo project. "Otherworld" is a fictional store. Prices, stats, rankings and the newsletter are placeholders, and nothing is sold or collected.
- The light novel titles and cover artwork belong to their respective authors and publishers and are shown for demonstration only.

## Author

**Vincent Aaron** — [github.com/vincent-aaron](https://github.com/vincent-aaron)
