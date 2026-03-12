# Huseyin Bicen - Personal Website

Live site: [https://www.huseyinbicen.com](https://www.huseyinbicen.com)

## Overview

Single-page personal website for Huseyin Bicen, focused on backend engineering and AI-era infrastructure messaging.

The site is built as a static `index.html` file with:
- custom CSS theme and panel-based layout
- animated canvas particle background
- live counters for life span and professional tenure
- dynamic footer year
- social links (LinkedIn, GitHub, Instagram, Email)

## Run Locally

Because this is a static page, you can open `index.html` directly in a browser.

If you prefer a local server:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## Key Dynamic Fields

All dynamic values are handled in the inline JavaScript inside `index.html`.

- Footer year:
  - `new Date().getFullYear()` populates `#yr`
- Professional experience text:
  - `#exp-years` is calculated from work start date (`2019-09-09 09:00:00`)
  - renders as `N+ years` when there is partial progress into the next year
- Life span and professional tenure counters:
  - updated every second via `tick()`
  - source dates:
    - birth date: `1996-06-13 09:00:00`
    - work start: `2019-09-09 09:00:00`

## Main File

- `index.html` - markup, styling, and scripts in one file

## Credits / Inspiration

- https://github.com/HasanNaser/My-Personel-Website
- https://codepen.io/franky/pen/LGMWPK
- https://github.com/JulianLaval/canvas-particle-network
