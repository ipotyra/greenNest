# GreenNest

A landing page for a fictional indoor plant shop, built with plain HTML and CSS.

## Preview

Open `index.html` in any browser — no build step or dependencies required.

## Structure

- **Header** — logo and navigation (Home, Shop, Care Guide, Blog, Contact)
- **Hero section** — headline, CTA button, and store stats (varieties, customers, deliveries, rating)
- **Why Shop section** — 4 selling points (delivery, support, plant guarantee, secure payments)
- **Featured Plants section** — grid of plant cards with images and names

## Tech

- Plain HTML5 + CSS3 (no frameworks, no JS)
- CSS Grid for the "Why Shop" and "Featured Plants" grids, Flexbox for header/hero
- Color palette based on green (`#2b5a3d`) and soft off-white backgrounds

## File structure

```
.
├── index.html
├── style.css
└── img/
    ├── Download.jpg          (hero background)
    ├── Download (2).jpg
    ├── Download (3).jpg
    └── Download (4).jpg
```

## Known issues

- **Image file names** — some images have spaces and long/inconsistent names (e.g. `Planta Bananeira Ravenala 18 Folhas Palmeira 310cm Folhagem.jpg`, `Download (2).jpg`). Recommended to rename to something consistent like `plant-1.jpg`, `plant-2.jpg`, etc.
- **Missing `alt` text** — all plant images have empty `alt=""` attributes; should be filled in for accessibility (e.g. `alt="Monstera Deliciosa"`).
- **`.icons` CSS class** — styled in `style.css` but not used anywhere in `index.html` (no icons in the nav).
- **No footer** — the page ends after the featured plants section; consider adding a footer with contact/social info.
- **Not fully responsive** — no media queries yet; the 4-column grids will break on smaller screens.

## Customize

- **Colors** — main green accent is `#2b5a3d`, used for logo, buttons, and headings
- **Content** — edit plant names/images directly in `index.html`
- **Layout** — grid columns are set via `repeat(4, 1fr)` in `.why-grid` and `.plant-grid`
