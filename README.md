# ⚔️ Epic Fury War Room — Iran Conflict Simulator 2026

Real-time barrel-by-barrel, country-by-country oil & gas war simulator.
Live market data · LNG crisis tracking · 11-country GDP impact · GDELT neutral news

## Quick Deploy (Free, 10 minutes)

### Step 1: GitHub repo
1. Go to github.com → New repository → name it `warroom`
2. Upload all files from this zip (drag & drop or `git push`)
3. Make sure `.nojekyll` and `.github/workflows/deploy.yml` are included

### Step 2: Enable GitHub Pages
1. Repo Settings → Pages → Source: **GitHub Actions**
2. First push triggers auto-deploy → live at `https://YOUR_USERNAME.github.io/warroom`

### Step 3: Custom domain ($12/yr, optional)
1. Buy domain at Namecheap/Porkbun (e.g. `epicfurysim.com`)
2. Add DNS record: `CNAME @ YOUR_USERNAME.github.io`
3. Edit `CNAME` file → replace with your domain
4. Repo Settings → Pages → Custom domain → enter it
5. ✅ Enable "Enforce HTTPS"

### Step 4: Ko-fi donations
1. Create account at ko-fi.com
2. In `index.html` find `ko-fi.com/warroomiransim`
3. Replace with your Ko-fi username
4. Post on LinkedIn/Twitter with a screenshot of the map

## File Guide

| File | Purpose |
|------|---------|
| `index.html` | Main simulator (self-contained, no build step) |
| `tests.js` | 41-test suite — runs in Node.js or browser |
| `test.html` | Browser test runner UI |
| `CNAME` | Custom domain (edit with your domain) |
| `.nojekyll` | Tells GitHub Pages to serve HTML directly |
| `.github/workflows/deploy.yml` | CI/CD — runs tests then deploys |

## APIs Used (all free, no key required)
- **Yahoo Finance** — live oil/gas/equity prices on load
- **GDELT Doc API** — neutral world news (toneabs<3 filter)

## Marketing (short window — conflict active now)
- LinkedIn post with map screenshot + "I built this"
- Reddit: r/geopolitics, r/worldnews, r/energy
- Twitter/X with #IranWar #EpicFury #OilCrisis tags
- Email to energy/defense journalists with link

## Test Suite
```bash
node tests.js
# Tests: 41 | Passed: 41 | Failed: 0
```

## Sources
All data points sourced to primary publications (EIA, IEA, Bruegel, Bloomberg,
CNN, Al Jazeera, JPost, CNBC, Foreign Policy). Links clickable inline in the UI.

## License
MIT — use freely, attribution appreciated
