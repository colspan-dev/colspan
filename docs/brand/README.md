# Colspan brand assets

The logo is the word set as a table: each letter sits in a cell, and the accent cell `o` spans two columns.

| File | Use |
| --- | --- |
| `colspan-logo-animated.svg` | Plays once: one cell divides, buds into the full logo and stops. README, landing hero. |
| `colspan-logo-animated-loop.svg` | Same animation on a loop. Loading and splash screens. |
| `logo-grid-black.svg`, `logo-grid-white.svg` | Static 4×2 logo for light and dark backgrounds. |
| `logo-row-black.svg`, `logo-row-white.svg` | Single-row logo for headers and small sizes. |
| `icon.svg` | 2×2 icon without cell numbers, readable down to 16 px. Source of `public/favicon.ico`. |

Animations use SMIL inside the SVG, so they play in `<img>` tags without JavaScript and switch to a dark palette with `prefers-color-scheme`.

Accent colour: `#6D5DFC`. Letters and cell numbers: JetBrains Mono (OFL), converted to outlines.
