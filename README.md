# My curriculum (HTML → PDF)

A single HTML page you can open in a browser and **save as PDF** — that’s the whole idea. No build step, no framework: one file, your CV. ;)

## What’s inside

- **`index.html`** — Self-contained résumé: structure, typography, and styles in one place.
- **Print layout** — `@media print` targets **A4**, strips screen-only chrome (shadows, page margins), and keeps header colors via `print-color-adjust` so the PDF looks like the page.

## Preview

Open `index.html` in any modern browser (double-click or drag the file into a window).

## Export to PDF

1. Use **Print** (`Ctrl+P` / `Cmd+P`).
2. Choose **Save as PDF** (or “Microsoft Print to PDF”, etc.).
3. Prefer **A4** if your print dialog lets you pick paper size (the CSS assumes A4).
4. Enable **background graphics** / **print backgrounds** if you want the navy header and accents to match the on-screen version.

That’s it — tweak the HTML, print again, ship the PDF.
