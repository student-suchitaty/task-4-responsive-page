# Task 4 – Make a Website Mobile-Friendly Using CSS Media Queries

A desktop-only hiking club page converted into a responsive, mobile-friendly layout using CSS media queries, built for the Web Development Internship (Elevate Labs).

## Before and after
- `desktop-only.css` – the original desktop-only version (fixed widths, no media queries)
- `style.css` – the responsive version used by `index.html`

## What I changed
| Problem in the desktop version | Fix in the responsive version |
|---|---|
| Fixed `width: 1000px` container | `width: 90%` with `max-width: 1000px` |
| Fixed `px` widths on hero columns and cards | `flex: 1` and CSS Grid with `1fr` columns |
| Fixed 480px SVG image | `max-width: 100%; height: auto` |
| `px` font sizes | `rem` units |
| Horizontal nav overflowed on phones | Nav stacks vertically below 768px |
| Three cards in a row | 3 columns, then 2 (≤992px), then 1 (≤768px) |
| Large 60px heading | Reduced to 2.25rem (≤768px) and 1.9rem (≤480px) |

## Breakpoints
- `max-width: 992px` – tablet
- `max-width: 768px` – mobile
- `max-width: 480px` – small phones

## Concepts used
Media queries, viewport meta tag, Flexbox, CSS Grid, relative units (`%`, `rem`), flexible images

## Screenshots

**Before – mobile (horizontal scrolling, content cut off)**
![Before mobile](screenshots/before-mobile.png)

**After – mobile**
![After mobile](screenshots/after-mobile.png)

**After – desktop**
![After desktop](screenshots/after-desktop.png)

## How to test
1. Open `index.html` with Live Server.
2. Press F12, then Ctrl+Shift+M for the device toolbar.
3. Choose a phone size (for example iPhone SE) or drag the width below 768px.
4. To see the "before" version, change `style.css` to `desktop-only.css` in the `<link>` tag of `index.html`.