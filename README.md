# XLSX Compare

A lightweight, zero-install browser tool for comparing two `.xlsx` files side by side — with row-level diffing, inline change highlighting, and an interactive grid.

## Features

- **Row-level diff** — auto-detects the unique key column(s) per sheet to correctly match rows across files, no manual config needed
- **Inline cell diff** — modified cells show `old → new` in a single cell instead of duplicating rows
- **3-tab view**
  - **Summary** — cards per sheet showing added / deleted / modified row counts, click to jump to grid
  - **Sheet Grid** — full data grid with green (added), red (deleted), yellow (modified) highlights
  - **All Changes** — flat filterable list of every change with old and new values
- **Interactive grid**
  - Lock columns left or right (sticky scroll) — click header to pin left, Shift+click to pin right
  - Lock rows — click row number to pin
  - Resize columns and rows by dragging edges
  - Hide unchanged rows/columns toggle
- **No install, no server** — open `index.html` directly in any browser

## Usage

1. Open `index.html` in a browser
2. Drop or select **File A** (original) and **File B** (modified)
3. Click **Compare**

## Files

| File | Purpose |
|------|---------|
| `index.html` | UI layout and styles |
| `script.js` | All comparison logic and rendering |

## Dependencies

- [SheetJS](https://sheetjs.com/) — loaded from CDN, no install needed
