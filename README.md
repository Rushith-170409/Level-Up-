# Level Up — installable web app

This folder contains a mobile-first PWA (Progressive Web App) prototype.

## Included
- `index.html` — full app UI and logic
- `manifest.json` — install metadata
- `service-worker.js` — offline app shell cache
- `icon.svg` — app icon

## Install on Android
A PWA needs to be served over HTTPS (or localhost) for installation and offline service-worker support. A ZIP opened directly from Downloads is not enough to install it as a PWA.

1. Upload the contents of this folder to a static HTTPS host (for example, a static site host).
2. Open the resulting HTTPS URL in Chrome on Android.
3. Open Chrome's menu and choose **Install app** or **Add to Home screen** (wording can vary).
4. Launch Level Up from the new home-screen icon.

## Data and backups
- Data is stored locally in the browser using `localStorage`; it is not synced across devices.
- Use **Data & settings → Export backup** to download a JSON backup.
- Use **Import backup** to restore it.
- Clearing browser data can erase unexported progress.

## Notes
XP ranges and some score measurement details are prototype defaults. The two quality scores are separate:
- Progress Quality: habit execution 30%, meaningful goal progress 35%, focused work 20%, consistency 15%.
- Day Quality: health & energy 30%, discipline & routines 20%, balance & well-being 15%, intentional use of time 35%.

No level-up rewards are included. Missed days do not remove XP; the app offers recovery challenges.
