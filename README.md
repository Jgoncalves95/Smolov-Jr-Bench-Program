# Smolov Jr. Bench Press Tracker

A mobile-first Progressive Web App (PWA) for tracking the Smolov Jr. bench press program.

Built as a single HTML file — no build tools, no frameworks, no dependencies. Deploy it anywhere and open it on your phone.

![Preview](https://img.shields.io/badge/1RM-280→315-red?style=for-the-badge)

## Features

- **Full Smolov Jr. program** — Weeks 1-3 with auto-calculated weights
- **Deload week** — Structured Week 4 recovery protocol
- **Max test day** — Warm-up ladder + 3 attempt structure
- **Rest timer** — Auto-starts on set completion with vibration alert
- **Progress tracking** — RPE logging, set completion, volume stats
- **Offline-capable** — Works without internet after first load
- **Add to home screen** — Feels like a native app on iOS/Android
- **Persistent state** — All progress saved to localStorage

## Deploy to GitHub Pages (free hosting)

### 1. Create a GitHub repo

```bash
git init
git add .
git commit -m "Smolov Jr. bench tracker"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/smolov-jr.git
git push -u origin main
```

### 2. Enable GitHub Pages

1. Go to your repo on GitHub
2. Click **Settings** → **Pages**
3. Under "Source", select **Deploy from a branch**
4. Select **main** branch, **/ (root)** folder
5. Click **Save**

Your app will be live at: `https://YOUR_USERNAME.github.io/smolov-jr/`

### 3. Add to your phone's home screen

**iPhone (Safari):**
1. Open the URL in Safari
2. Tap the **Share** button (box with arrow)
3. Scroll down and tap **Add to Home Screen**
4. Tap **Add**

**Android (Chrome):**
1. Open the URL in Chrome
2. Tap the **⋮** menu
3. Tap **Add to Home screen** or **Install app**
4. Tap **Add**

The app will now appear on your home screen and open in full-screen mode like a native app.

## Customization

Tap the **⚙** gear icon in the app to change:
- **Current 1RM** — all weights recalculate automatically
- **Goal 1RM** — updates the max test day targets
- **Weekly increment** — 10-20 lbs (default: 10)
- **Rest timer** — seconds between sets (default: 180)

## Program Structure

| Day | Sets × Reps | % of 1RM | @ 280 1RM |
|-----|-------------|----------|-----------|
| Monday | 6 × 6 | 70% | 195 lb |
| Wednesday | 7 × 5 | 75% | 210 lb |
| Friday | 8 × 4 | 80% | 225 lb |
| Saturday | 10 × 3 | 85% | 240 lb |

Add 10 lbs to all working weights each week.

## Tech

- Single `index.html` — no build step, no bundler
- Pure HTML/CSS/JS — zero dependencies
- localStorage for state persistence
- CSS custom properties for theming
- PWA manifest for home screen install

## License

MIT — do whatever you want with it.
