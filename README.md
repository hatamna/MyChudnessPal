# MyChudnessPal

A reverse fitness tracker built in a couple of hours for a hackathon. Instead of rewarding steps and productivity, MyChudnessPal gamifies your **Stagnation Index**—rewarding stillness, lying down, and doomscrolling while penalizing walking and studying.

## Features

- **Live Sensor Tracking:** Uses device accelerometer data to track time unmoved, count steps (`-8 pts`), and detect lying-down "bedrot" posture (`10x` rate).
- **Protected Hours & Warnings:** Set custom School/Work and Sleep schedules. Screen time during protected hours triggers a red warning alert, haptic feedback, shaking UI islands, and a `10x` multiplier (paused automatically when walking).
- **App Activity Tracker:** Adds points for YouTube/Instagram and deducts points for Pulse/Classroom, with support for silent background triggers via `ntfy.sh` + MacroDroid.
- **Live Room Leaderboards:** Create a persistent account and join a 4-digit room code to sync scores live with friends over retained MQTT WebSockets.
- **Installable PWA:** Monochrome liquid-glass UI styled with Doto typography. Installs directly to iOS/Android home screens in standalone mode.

## Quick Start

Zero build steps or backend setup required:

1. Deploy the project folder (`index.html`, `manifest.json`, `sw.js`, `icon-192.png`, `icon-512.png`) to any HTTPS static host (GitHub Pages, Netlify Drop, Vercel).
2. Open the URL on mobile and select **Install App / Add to Home Screen** to hide the browser bar.
3. Tap the top-right status chip to enable motion sensors.
