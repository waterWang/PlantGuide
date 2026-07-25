# PlantGuide Web Demo

A lightweight, self-contained web UI for browsing and filtering plant species with care cards.

## Features

- **Tag Picker** — Filter 160+ plant species by categories: light requirements, water needs, indoor/outdoor, care level, style, type, features, and leaf characteristics
- **Care Cards** — Click any plant to see its full care profile: light, water, soil, humidity, temperature, fertilizer, toxicity, common issues, and care tips
- **Search** — Search by common name, scientific name, or species ID
- **Responsive** — Works on desktop and mobile

## Quick Start

Open `index.html` in any modern browser — no server, no build tools, no dependencies.

```bash
# Just open the file
open index.html
```

Or serve with any HTTP server:

```bash
python3 -m http.server 8000
# Open http://localhost:8000
```

## Structure

```
web/
├── index.html    # Main entry point
├── style.css     # Styles (Inter font, responsive layout)
├── app.js        # App logic (tag filtering, search, modal)
├── data.js       # Species data (160 species, auto-generated)
└── README.md     # This file
```

## Data

The species data is generated from `data/species/*.json` using:

```bash
python3 scripts/generate-web-data.py
```

## Screenshots

![Desktop view](screenshots/desktop.png)
![Mobile view](screenshots/mobile.png)
![Care card modal](screenshots/care-card.png)