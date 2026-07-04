# SimCrate

Landing page for **SimCrate** — home flight simulator rentals for student pilots.

Rent a complete physical flight simulator by the month: delivered, set up, and
configured to match your training aircraft. Launching in Dallas–Fort Worth in
fall 2026.

## About

This repository holds the SimCrate marketing site — a single, self-contained
`index.html` with no build step and no dependencies. It covers the rig, how the
rental works, pricing tiers (Standard and BATD Pro), at-home requirements, an
FAQ, and a waitlist signup.

## Structure

| File         | Purpose                                            |
| ------------ | -------------------------------------------------- |
| `index.html` | The entire landing page (HTML, CSS, and JS inline) |
| `images/`    | Rig photos referenced by the gallery (optional)    |

## Running locally

No build tooling is required. Open the file directly:

```sh
open index.html
```

Or serve it with any static server:

```sh
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Design

- **Type:** Bricolage Grotesque, Inter, and IBM Plex Mono (loaded from Google Fonts)
- **Palette:** clean white background with an aviation-inspired accent set
  (magenta, chart blue, amber)
- **Theme:** instrument-panel and checklist motifs throughout (attitude
  indicator, METAR ticker, spec sheets)

## Waitlist form

The email capture is currently a front-end placeholder that logs to the console.
Before launch, wire the form in `index.html` to a real endpoint (e.g. Formspree
or a serverless function). Look for the `wireForm` handler and the `TODO`
comment near the bottom of the file.
