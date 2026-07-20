# C'mon Bell! 🎣

**A modern, real-time fishing journal and trip planner built for serious anglers and fishing groups.**

C'mon Bell! turns your fishing adventures into a beautiful, collaborative digital logbook. Whether you're fishing solo or with a group of buddies, the app keeps everyone in sync and helps you fish smarter with data-driven insights.

---

## ✨ Key Features

### 📊 **Real-Time Collaboration**
- All group members see new catches instantly
- Powered by Firebase Firestore — no refresh needed
- Changes sync automatically when back online

### 🎣 **Rich Catch Logging**
- Species (with extensive freshwater & saltwater options)
- Length, weight, date, time
- GPS coordinates (with one-tap location capture)
- Weather conditions & temperature
- Lure / bait used
- Photo upload (stored securely)
- Detailed notes
- Link catches to saved fishing spots

### 📍 **Fishing Spots Management**
- Save your favorite holes with name, coordinates, water type, access method, and tips
- Visual map view with Leaflet
- Automatic catch count per spot

### 🌙 **Solunar & Weather Intelligence**
- Accurate solunar calculations (major & minor periods, moon phase, illumination)
- 7-day forecast strip on the home screen
- Full daily breakdown with sunrise/sunset
- Live local weather with hourly forecast
- Trip planner — check any location and date

### 📈 **Stats & Insights**
- Group leaderboard (most catches, biggest fish)
- Top species, lures, and spots
- "Fish Intel" section showing best times of day and proven lures per species
- Personal and group pattern recognition

### 🗂️ **Organized Views**
- Catch Log with powerful search & filters
- Trip grouping (automatic daily summaries)
- Dedicated Tactics page with practical recommendations
- Beautiful, mobile-optimized interface

---

## 🎯 Who Is This For?

- Weekend anglers who want to remember what worked
- Serious fishermen building a personal knowledge base
- Fishing groups, clubs, or guides who share data
- Anyone who enjoys tracking progress and improving over time

---

## 🚀 Getting Started

1. **Download** the single file: `the-hole-v5.html`
2. **Open** it in any modern browser (Chrome, Safari, Firefox)
3. **Enter your name** when prompted (stored only on your device)
4. **Start logging** your first catch!

> **Tip**: Add the app to your home screen (PWA) for the best mobile experience.

### Offline Mode
You can log catches without internet. They will sync automatically when connection is restored.

---

## Technical Details

- **Single HTML file** — no installation, no server required
- **Frontend**: Vanilla JavaScript, Tailwind-inspired custom CSS
- **Backend**: Firebase (Firestore + Storage)
- **Maps**: Leaflet + OpenStreetMap
- **Weather**: Open-Meteo API (free, no key needed)
- **Solunar**: Pure client-side astronomy calculations

### Firebase Setup (Optional)
The app includes a default Firebase project for quick testing. For production use with your group:
1. Create a new Firebase project
2. Replace the `firebaseConfig` object in the script
3. Enable Firestore and Storage

---

## Customization

The app is very easy to personalize:
- Modify color scheme in `:root` CSS variables
- Add/remove species or lures in the form dropdowns
- Extend the `GENERIC_INTEL` object for more species
- Tweak layouts and components directly in the HTML/CSS

---

## Screenshots

*(Add screenshots here when available)*

- Dashboard with weather & solunar
- Catch logging modal
- Spot map view
- Leaderboard & stats
- Fish Intel cards

---

## Roadmap / Future Ideas

- Export data (CSV / PDF)
- Advanced analytics & charts
- Offline-first improvements with IndexedDB
- Species-specific pattern recognition
- Community lure database (optional)

---

## License

This project is open for personal and group use. Feel free to fork, modify, and improve it.

---

## Feedback & Support

Made with passion for fishing and good times on the water.  

If you have suggestions, bug reports, or want to contribute improvements — feel free to reach out!

---

**Tight lines and C'mon Bell!** 🎣

*May your logs be long and your fish stories even longer.*
