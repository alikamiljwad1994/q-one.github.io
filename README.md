# Q-One v0.3 — Advanced Motion Design Engine

Q-One v0.3 expands the design-first prototype with a richer icon, typography, divider, motion, and activity-template system.

## Run
Open `index.html`, then enter the studio through `dashboard.html`. For best results, serve the folder with a local web server so browser storage and external font/icon assets behave consistently.

Example:

```bash
python -m http.server 8000
```

Then visit `http://localhost:8000`.

## Lucide
The full Lucide UMD library is loaded from the official package CDN. The Block Editor exposes a search picker that searches the library index and assigns a Lucide icon per link. If the page is opened without Internet access, saved content still works but remote Lucide/font assets may not load until a connection is available.

## Bilingual fonts
The design engine includes these Arabic/English-capable families: Readex Pro, Cairo, Tajawal, IBM Plex Sans Arabic, Noto Sans Arabic, Alexandria, Noto Kufi Arabic, Changa, and El Messiri, plus System UI.

## Motion system
Two independent layers are available:

- Continuous motion: None, Subtle, Float, Glow, Breathe, Drift.
- Scroll reveal: None, Fade Up/Down/Left/Right, Zoom, Blur, Soft Flip, Bounce.

Duration and stagger are configurable. `prefers-reduced-motion` is respected.

## Animated activity templates
19 lightweight animated scene presets are included: restaurant, cafe, bakery, medical, dental, beauty, fashion, real estate, automotive, fitness, education, technology, gaming, photography, travel, ecommerce, business, events, and hotel.

These are generated as lightweight SVG/CSS-style motion layers rather than heavy GIF/video backgrounds.

## Dividers
- Automatic divider between link cards.
- Manual Divider block inserted anywhere in the content order.
- Styles: Solid, Dashed, Dotted, Gradient, Glow.
- Adjustable opacity and width.

## State
Design state is stored under `qone-state-v03` in LocalStorage. Existing v0.2 state is migrated automatically. See `design-schema.json`.
