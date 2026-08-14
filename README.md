# C'mon Bell! 🎣

*Fish. Log. Catch. Repeat.*

A single-page fishing companion app for logging catches, tracking spots, planning trips around solunar and weather conditions, and keeping your whole fishing group in sync — in real time.

---

## Features

### 🏠 Dashboard
- **Live status ticker** — a rotating banner that surfaces whatever's most relevant right now: the next major/minor bite window, current weather, your latest catch, your hottest spot, this week's catch count, personal bests, catching streaks, favorite lure, species tally, moon phase, sunrise/sunset countdown, top spot this month, and rotating fishing tips. Tap any message to jump straight to the related tab.
- **Local weather widget** — current conditions for your location.
- **Solunar widget** — today's day-quality rating and upcoming bite windows at a glance.
- **7-day outlook strip** — a scrollable preview of the week ahead, with a link to the full forecast.
- **Quick stats & quick actions** — at-a-glance totals and one-tap shortcuts (e.g. jump to your latest catch).
- **Recent pattern & spot heat** — mini summaries of what's been biting and where, with links to dig deeper in Stats and Spots.

### 🐟 Catch Log
- Log a catch with species, length, weight, angler, lure, weather, temperature, GPS coordinates (auto-filled via "Use My Location"), a photo, and free-form notes.
- Full-text search across species, spot, angler, lure, and notes.
- Filter by angler or species.
- Tap any catch to view details full-screen, including a pinch/double-tap-to-zoom photo lightbox.
- Edit or delete any entry.

### 📅 Trips
- Catches are automatically grouped into trips by day, across the whole group — no manual trip creation needed.

### 🌙 Solunar Forecast
- 7 days of day-quality ratings and major/minor bite windows, calculated from moon phase and position.
- Sunrise and sunset times for each day.

### 🗓 Trip Planner
- Search any location worldwide and pick a date (including future dates) to preview weather and solunar conditions before you go — great for planning ahead of a trip to unfamiliar water.
- Automatically re-checks the forecast if you change the date after picking a location.

### 📍 Fishing Spots
- Save spots with names and notes.
- Interactive map view of all your saved spots.
- See how many catches came from each spot to spot your most productive water.

### 📊 Stats
- Group-wide breakdowns: top species, biggest catch, most active angler, spots used, and more.

### 🎯 Tactics
- Simple, practical heuristics generated from your *own* logged history — best weather conditions, most productive lure, most frequent species, most active angler, and your best-performing spot.

### 🐟 Fish Intel
- Per-species activity patterns (best time of day, top lures) built from your group's own catch data, blended with general species knowledge when you don't have enough catches logged yet for a given species.

### 👥 Real-Time Group Sync
- All catches and spots sync live across every device via Firebase — no refresh needed.
- When a teammate logs a catch, everyone else gets an instant on-screen alert (e.g. *"🎣 Alex just landed a Largemouth Bass · 4.1 lb!"*).
- Automatic offline detection — the app clearly flags when changes are only saved locally and haven't synced yet.

### ✨ Splash Screen
- An animated intro plays on launch, blended seamlessly into the app's background color.

---

## Tech Stack

- **Frontend:** Vanilla HTML, CSS, and JavaScript — no build step, no framework, a single self-contained file.
- **Data & sync:** Firebase Firestore (real-time database) and Firebase Storage (catch photos).
- **Weather & astronomy:** Open-Meteo API for forecasts; solunar/moon-phase/sunrise-sunset calculations run locally in-browser.
- **Maps:** Leaflet.js for the interactive spots map.

## Deployment

This app ships as a single HTML file with everything (styles, scripts, and images) bundled inline.

1. Upload the file to your GitHub repository, **named exactly `index.html`**, at the root of the branch your GitHub Pages site serves from.
2. GitHub Pages will redeploy automatically within about a minute.
3. Open your Pages URL (e.g. `https://yourname.github.io/yourrepo/`) on any device — desktop or mobile.

No installation, build process, or server required.
