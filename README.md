# CP · Road to 2200

> A competitive programming study guide + Codeforces profile tracker. Deploy it on GitHub Pages in 2 minutes, track your progress across sessions.

![preview](https://img.shields.io/badge/deploy-GitHub%20Pages-7c6aff?style=flat-square) ![single file](https://img.shields.io/badge/single%20file-HTML-22d3ee?style=flat-square) ![no backend](https://img.shields.io/badge/backend-none-4ade80?style=flat-square)

---

## What's inside

**Dashboard tab**
- Live CF profile card — enter any handle to load rating, solved count, contest history
- +/− delta for every contest (Faceit-style)
- Streak dots (green = win, red = loss)
- Rating tier roadmap — unlocked/current/next tiers highlighted dynamically
- Tag frequency data from 4800+ CF problems (1800–2200)

**Study Guide tab**
- 17 topics: Binary Search → DP Optimization (CHT / Aliens trick)
- 120+ hand-picked problems with ratings (CSES + CF)
- C++ templates for each topic
- Mark problems solved, mark topics Done
- Progress bar across all 120+ problems

**Progress storage**
- Saves to `localStorage` — persists across page reloads on the same device
- Export as JSON → import on another device
- Reset button if you want a clean slate

---

## Deploy to GitHub Pages (2 min)

### Option A — Fork & enable Pages (recommended)

1. Click **Fork** (top right on this repo)
2. Go to your fork → **Settings** → **Pages**
3. Under *Source*, select **Deploy from a branch**
4. Choose branch `main`, folder `/ (root)`
5. Click **Save**
6. Wait ~60 seconds → your site is live at:
   ```
   https://<your-username>.github.io/<repo-name>/
   ```

### Option B — New repo from scratch

```bash
# 1. Create a folder and put index.html inside
mkdir cp-guide && cd cp-guide
# (copy index.html here)

# 2. Init git and push
git init
git add index.html README.md
git commit -m "init"
git branch -M main
git remote add origin https://github.com/<you>/<repo>.git
git push -u origin main

# 3. Enable Pages in GitHub Settings → Pages → main / root
```

### Option C — GitHub CLI (fastest)

```bash
gh repo create cp-guide --public --source=. --remote=origin --push
# then enable Pages in repo Settings
```

---

## Customize for your handle

The default handle is `b1rr0`. To change it, open `index.html` and find:

```html
<input type="text" id="cfHandle" placeholder="CF handle…" value="b1rr0"/>
```

Replace `b1rr0` with your own handle. Or just type it in the search box at runtime — it loads dynamically from the CF API.

---

## How progress is stored

| Storage | Where | Persists |
|---------|-------|---------|
| `localStorage` | Your browser | ✅ Across reloads on same device |
| Export JSON | File on disk | ✅ Manually, cross-device |
| GitHub | Not used | — No backend needed |

To sync between devices: use **Export JSON** on device A → **Import JSON** on device B.

---

## Tech stack

- Pure HTML + CSS + JS — zero dependencies, zero build step
- Codeforces public API (`user.info`, `user.rating`, `user.status`)
- Google Fonts (JetBrains Mono + Syne)
- `localStorage` for persistence

---

## Rating tier thresholds (CF)

| Tier | Range | Color |
|------|-------|-------|
| 🌱 Newbie | 0–1199 | Gray |
| 📗 Pupil | 1200–1399 | Green |
| 🔵 Specialist | 1400–1599 | Teal |
| ⚡ Expert | 1600–1899 | Blue |
| 💜 Candidate Master | 1900–2099 | Purple |
| 🔥 Master | 2100–2299 | Orange |
| ⭐ International Master | 2300–2399 | Orange |
| 👑 Grandmaster+ | 2400+ | Red |

---

## Forking tips

- Change the target rating (currently 2200) by finding `2200` in the JS and updating `const TARGET=2200`
- Add your own problems to any topic section — copy a `.pr` row inside any `.pc2` block
- The CF API is public and rate-limited at ~5 req/sec — no key needed

---

## License

MIT — fork, modify, deploy freely.
