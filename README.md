# Tunnel Dash 🚇 — Subway Surfers-style Endless Runner

Pure **HTML + CSS + JS** (single file, no framework, no build step) endless runner:
3 lanes, jump/slide/dodge trains, collect coins, speed badhti jaati hai jaise jaise
distance cover hota hai. `index.html` kholo, browser me chal jayega.

## Controls
- **← / →** — lane switch
- **↑ / Space** — jump
- **↓** — slide
- Mobile: swipe left/right/up/down

---

## 🗺️ Roadmap (game improve karne ke liye)

### Phase 1 — Polish current version
- [ ] Character sprite / simple pixel-art animation add karo (abhi geometric shapes hain)
- [ ] Sound effects: jump, coin collect, crash (Web Audio API ya `<audio>` tags)
- [ ] Background music toggle button
- [ ] Local leaderboard (top 5 scores, `localStorage` already best score store kar raha hai)

### Phase 2 — Gameplay depth
- [ ] Power-ups: magnet (auto coin collect), shield (1 free hit), score multiplier
- [ ] Multiple themes (day tunnel, night tunnel, city rooftop) — random ya score-based unlock
- [ ] Difficulty curve tune karo (obstacle spawn rate, speed ramp)
- [ ] Combo system: consecutive coin pickups par bonus

### Phase 3 — Mobile & PWA
- [ ] `manifest.json` + service worker add karke installable PWA banao
- [ ] Offline support
- [ ] Touch button overlay (on-screen jump/slide buttons) for better mobile UX

### Phase 4 — Backend / online features (optional)
- [ ] Firebase / Supabase se global leaderboard
- [ ] Simple auth (Google sign-in) score save karne ke liye
- [ ] Daily challenge seed (same obstacle pattern for everyone that day)

### Phase 5 — Deployment
- [ ] GitHub Pages / Vercel / Netlify par deploy karo (free hosting)
- [ ] Custom domain (optional)

---

## 🚀 GitHub par push kaise karo

Assuming git already installed hai aur GitHub account bana hua hai.

### 1. Local repo banao
```bash
cd subway-runner
git init
git add .
git commit -m "Initial commit: Tunnel Dash endless runner"
```

### 2. GitHub par naya repository banao
- github.com par login karo → **New repository** click karo
- Name do (e.g. `tunnel-dash`), public/private choose karo, **README add mat karo** (already local hai)
- **Create repository** click karo

### 3. Local repo ko GitHub se connect karo
GitHub jo commands dikhayega repo banane ke baad, waise hi:
```bash
git branch -M main
git remote add origin https://github.com/<your-username>/tunnel-dash.git
git push -u origin main
```

### 4. Future changes push karne ke liye
```bash
git add .
git commit -m "describe your change here"
git push
```

### 5. Free hosting — GitHub Pages (recommended for this game)
1. GitHub repo → **Settings** → **Pages**
2. Source: **Deploy from a branch** → Branch: `main`, folder: `/ (root)` → **Save**
3. 1-2 min baad game live hoga: `https://<your-username>.github.io/tunnel-dash/`

### 6. Alternative — Vercel / Netlify (1-click deploy)
- Netlify: repo import karo, build command khaali chodo, publish directory `/` set karo
- Vercel: repo import karo, framework "Other" select karo — static HTML detect ho jayega

---

## 📁 Project structure
```
subway-runner/
├── index.html   # Game — HTML + CSS + JS sab isi file me
└── README.md    # Ye file
```

Simple rakha gaya hai taaki GitHub Pages par bina kisi build step ke directly chal jaye.
