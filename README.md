# C'mon Bell! 🎣

A single-file, mobile-first fishing journal — log catches and trips, track your favorite spots, and plan around solunar and weather conditions. Built as one self-contained HTML file with Firebase for shared, real-time sync between anglers.

## Features

**Logging**
- **Catches** — species, weight/length, lure, angler, conditions, GPS, and photos, tied to a spot and/or trip.
- **Trips** — group catches from a single outing together, with a per-trip recap of who caught what.
- **Spots** — save named locations with notes and coordinates; view them on a heatmap of activity.

**Planning & conditions**
- **Forecast** — a 7-day outlook combining solunar major/minor bite windows, sunrise/sunset, moon phase, and daily weather (high/low, condition, wind) for your current location.
- **Trip Planner** — search any location and date (up to 30 days out) and get the same solunar + weather breakdown before you head out.
- **Dashboard** — an at-a-glance home screen: local weather, today's solunar summary, your latest catch, recent catch patterns, and a spot activity heatmap.

**Insights**
- **Stats** — personal catch history broken down over time.
- **Tactics** — bait and lure suggestions.
- **Fish Intel** — per-species best times-of-day and top lures, drawn from your own logged catches where available, falling back to general guidance otherwise.

**Sync**
- Catches, trips, and spots sync in real time through Firestore, so everyone logging against the same app instance sees each other's data.
- Catch photos upload to Firebase Storage.

## Navigation

A single-row bottom nav — **Home, Catches, Spots, More** — plus a floating **Log Catch** button. **More** opens a sheet with the rest: Trips, Forecast, Planner, Stats, Tactics, and Fish Intel.

## Design

Warm "tackle-box logbook" theme — olive and moss backgrounds, brass accents, and parchment-toned cards. Baloo 2 for headlines, Quicksand for body text.

## Tech

- Single `.html` file — no build step, no framework. Vanilla JS, CSS custom properties for theming.
- **Firebase** (Firestore + Storage, compat SDKs) for data sync and photo storage.
- **Leaflet** for the spot map.
- **Open-Meteo** (no API key required) for weather forecasts and location geocoding.
- Solunar and sun-time calculations are computed client-side from latitude/longitude and date.

## Setup

This is a static file — host it anywhere that serves plain HTML (GitHub Pages, Netlify, Firebase Hosting, etc.).

1. Create a Firebase project with **Firestore** and **Storage** enabled.
2. Replace the `firebaseConfig` object near the top of the `<script>` section with your own project's config (found in Firebase Console → Project Settings → General).
3. Set Firestore and Storage security rules to match how open you want catch/spot data to be between users — the app itself doesn't gate access, so rules are your access control.
4. Deploy the file to your host of choice.

> Note: Firebase web config values (including the `apiKey`) are safe to expose client-side — they identify your project, not authenticate requests. Access control is enforced by your Firestore/Storage security rules, not by keeping this config secret.

## Installing as an app

The page includes `apple-mobile-web-app-capable` meta tags, so on iOS you can add it to your home screen (Share → Add to Home Screen) for a chrome-less, app-like experience. There's no offline support yet — an active connection is required for weather, sync, and maps.

## Known limitations

- No offline mode / service worker — logging catches requires a live connection to Firestore.
- No authentication — anyone with the hosted link can read and write data, scoped only by your Firestore/Storage rules.
- Desktop layout (≥720px wide) hides the bottom navigation entirely; this app is designed and tested for mobile-width screens.
