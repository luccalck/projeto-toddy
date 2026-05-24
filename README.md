# Projeto Toddy

Fictional institutional website for the Toddy brand, developed as an ADS project — SENAI.

## Stack

- Static HTML
- Tailwind CSS (via CDN)
- Vanilla JavaScript
- `.mp4` videos with scroll-controlled playback and autoplay loops

## Structure

```
projeto-toddy/
├── index.html      # Single page (static SPA)
└── video/          # Product videos and images
    ├── TODDYUSAR_scrub.mp4    # Hero — scroll-controlled
    ├── ToddyFullFrames.mp4    # Toddy Original — autoplay loop
    └── toddyblack169.png      # Toddy Dark
```

## Features

- Hero with scroll-controlled video (scrub)
- Bidirectional fade-in/out animations on scroll
- 3 products + 3 combos with pricing
- Drawer cart with quantity, total, and `localStorage` persistence
- Simple login (name + email) with validation
- Order confirmation with auto-generated reference number
- Logout shown on the navbar when logged in
- Newsletter with email validation
- Visually hidden scrollbar, smooth scrolling page-wide

## How to run locally

Because of the videos, you must serve via HTTP (don't open the file directly):

```bash
python -m http.server 5181
# open http://localhost:5181
```

## Deploy

Static site — works out of the box on Vercel, Netlify or GitHub Pages with no build step.
