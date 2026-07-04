# 6-Color Palette Generator

A small browser-based tool that generates a 6-color palette from a single input color using a seeded algorithm and OKLCH color manipulation.

This is a **prototype / experimental tool**, not a strict color harmony system.

---

## Features

- Generate a 6-color palette from a single HEX input
- Accepts:
  - Custom HEX color (e.g. #39a78e)
  - Random fallback color if input is invalid
- Deterministic output using a seeded RNG (same input = same palette)
- Uses OKLCH-based color transformations for more perceptual consistency
- Simple copy-friendly output format for design tools (like Krita)

---

## How to Use

1. Open the HTML file in your browser
2. Enter a HEX color (optional)
3. Click **Generate Palette**
4. View:
   - Visual swatches
   - Copy-ready HEX list below

---

## How It Works

The palette generation is based on:

- A **seeded pseudo-random generator** to keep results consistent
- Conversion between **RGB ↔ OKLCH color space**
- Controlled hue offsets:
  - Analogous colors
  - Complementary contrasts
  - Accent shifts
- Lightness and chroma adjustments tied to the base color

The first color is always the input color, and the remaining five are derived variations.

---

## Disclaimer

This palette generator is an experimental algorithm and should not be treated as a strict rule for what “good” color combinations are.
It provides **starting points for creative work**, not definitive design rules. Feel free to adjust, remix, or ignore any generated palette.

---

## Tech Used

- Vanilla JavaScript
- HTML + CSS (no frameworks)
- OKLCH color space math
- Custom seeded RNG

---

## License
This project is for **personal, non-commercial use only**.
You may view and modify the code for learning or personal projects, but you may not use it commercially or redistribute it.
