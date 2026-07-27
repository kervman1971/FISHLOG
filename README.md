# C'mon Bell! 🎣

A single-page web app fishing log — track catches, spots, weather, and stats, all from your phone.

Built by **KSM Studios**.

## What it does

- **Home** — dashboard with recent activity, quick stats, and a forecast preview at a glance.
- **Catches** — log your catches with species, weight, length, bait, and location.
- **Spots** — save and revisit your favorite fishing spots on a map.
- **Trips** — plan and track fishing trips.
- **Forecast** — check weather and conditions to help decide when to fish.
- **Planner** — schedule upcoming trips.
- **Stats** — dive into your fishing history and trends over time.
- **Tactics** — bait and technique tips.
- **Fish Intel** — reference info on species.

## Tech

- Single HTML file — no build step, no install. Just open it in a browser.
- **Firebase** (Firestore + Storage) for saving catches, photos, and spots to the cloud.
- Data persists across devices via Firebase, with a few local preferences (like your name) stored in `localStorage`.
- Fully responsive, mobile-first design with a bottom tab bar for navigation.

## Getting started

1. Open `the-hole-v6.html` in a browser (mobile or desktop).
2. Tap **Log Catch** to record your first catch, or explore the tabs via the bottom nav / "More" menu.
3. Your data syncs automatically to the app's Firebase backend.

## Notes

- This is a self-contained prototype — all markup, styles, and logic live in one HTML file for easy sharing and iteration.
- Color theme and branding (logo, header) can be adjusted directly in the `<style>` section at the top of the file.
