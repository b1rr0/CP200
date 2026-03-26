# CP · Road to 2200

> Competitive programming study guide + Codeforces profile tracker + cheatsheet with templates for C++, Java, Python.

![deploy](https://img.shields.io/badge/deploy-GitHub%20Pages-7c6aff?style=flat-square) ![single file](https://img.shields.io/badge/single%20file-HTML-22d3ee?style=flat-square) ![no backend](https://img.shields.io/badge/backend-none-4ade80?style=flat-square)

## Features

### Dashboard
- Live CF profile — enter any handle to load rating, contests, solved count
- Rating history sparkline + contest deltas (green/red)
- Streak tracker (wins/losses in a row)
- Rating tier roadmap with current/next tier highlighting
- Key stats: CF Rating, Solved, Contests, Max Rating

### Study Guide
- 24 topics from Implementation (800) to DP Optimization (2200)
- 248+ hand-picked problems (CF + LC + CSES) with ratings
- Theory & resources per topic (cp-algorithms, CF EDU, video courses)
- Mark problems solved, mark topics Done
- Progress bar across all problems
- EN/UA language switch

### Cheatsheet & Templates
- **Codeforces templates** for C++, Java (FastScanner), Python — one-click copy
- **Language-specific tips** (12 per language) — switch between C++ / Java / Python
- **Data structures table** — side-by-side comparison across all 3 languages (14 structures with complexity notes)

### Progress
- Saves to `localStorage` — persists across reloads
- Reset button for clean slate

---

## Deploy (2 min)

### Fork & enable Pages
1. **Fork** this repo
2. Settings → **Pages** → Branch: `main`, folder: `/ (root)` → **Save**
3. Wait ~60s → live at `https://<username>.github.io/CP200/`

### From scratch
```bash
git clone https://github.com/b1rr0/CP200.git
cd CP200
# edit index.html if needed
git push
```

---

## Customize

Change default handle — find in `index.html`:
```html
<input type="text" id="cfHandle" value="b1rr0"/>
```
Or just type any handle in the search box at runtime.

---

## Tech

- Pure HTML + CSS + JS — zero dependencies, zero build
- Codeforces API (`user.info`, `user.rating`, `user.status`)
- Google Fonts (JetBrains Mono + Syne)
- `localStorage` for persistence

---

MIT — fork, modify, deploy freely.
