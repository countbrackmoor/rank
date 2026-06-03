# Rank

A pairwise comparison prioritizer. Give it any list — tasks, movies, goals, decisions — and it ranks everything through head-to-head choices until a clear order emerges.

Live at **[gorgon.live/rank](https://gorgon.live/rank)**

---

## How it works

1. **Enter your list** — one item per line, minimum two items
2. **Make choices** — two options appear at a time; pick whichever matters more
3. **See results** — items are ranked by total wins across all comparisons

Every unique pair is compared exactly once. For *n* items that's *n(n−1)/2* comparisons total, shown in a live progress bar. A running standings table updates after each pick so you can see the order taking shape as you go.

---

## Features

- **Pairwise scoring** — no guessing at relative weights; just binary choices
- **Live standings** — ranking updates in real time during comparison phase
- **Tie handling** — items with equal wins are flagged as tied in the final results
- **Edit & restart** — return to the list entry phase with your items preserved, or wipe everything and start fresh
- **No backend** — pure HTML/CSS/JS, no accounts, no data leaves your browser

---

## Usage

Open `index.html` directly in a browser or serve via any static host. No build step, no dependencies beyond Google Fonts (Barlow Condensed, Karla, DM Mono via CDN).

The gorgon.live nav bar (`← gorgon.live`) loads via `../nav.js` when served under the domain. It silently fails if the file is absent — no errors, no broken layout.

---

## Files

| File | Purpose |
|---|---|
| `index.html` | The entire tool — HTML, CSS, and JS in one file |
| `README.md` | This file |

---

## Stack

Pure HTML · CSS · Vanilla JS · Google Fonts CDN
