# Changelog — Rank

Pairwise comparison prioritizer. Repo: `countbrackmoor/rank`.

---

## 2026-06-13 — Export functionality

### Added
- **Copy list** button on results phase — copies ranked items to clipboard
- **Export CSV** button — downloads `rank-results.csv` with proper quoting (handles commas and embedded quotes in item names)
- **Include metrics** checkbox above the action row — unchecked by default, DM Mono styling, lime green when checked
  - With metrics on: copy output is tab-separated `Rank\tItem\tWins`; CSV columns are `Rank,Item,Wins`
  - With metrics off: items only (copy) or single `Item` column (CSV)
- Both buttons flash green "✓" on success

---

## 2026-06-13 — Initial integration into gorgon.live

### Added
- `nav.js` integration via `../nav.js` script tag with `onerror="void 0"` silent fail
- `README.md` covering algorithm, features, usage, file table, and stack

### Changed
- All dark-on-black font colors lifted for readability against the black background:
  - `#2e2a26` / `#302c28` → `#5e5a54`
  - `#3a3530` → `#6a6460`
  - `#4a4238` → `#7a7268`
  - `#5a5248` → `#8a847a`
- Lime green `#c8f72a` accent and `#eae4d4` foreground text preserved

---

## Earlier — Initial tool (baseline)

Tool existed prior to integration. Established before this log:

- Single-file `index.html` (HTML + CSS + JS)
- Three-phase flow: list entry → pairwise comparison → results
- Every unique pair compared exactly once (`n(n-1)/2` total)
- Live progress bar and live standings table during comparisons
- Tie handling for items with equal win counts
- Edit & restart (preserves list) and full wipe options
- Barlow Condensed, Karla, DM Mono via Google Fonts CDN
- No backend, no accounts, no data leaves the browser

No reliable record of the initial build's date.
