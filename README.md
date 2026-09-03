# Pulse — Habits & Workouts PWA

A mobile-first installable web app for personal habits, streaks, workouts and milestone rewards.

## Features
- Your 13 starter habits
- Per-habit custom days of week
- Daily scheduled-task completion
- Perfect Day marker when every scheduled task is complete
- Individual habit streaks + Perfect Day streak
- Built-in daily Bible verse
- Day-specific workout plan with YouTube demo searches
- Workout completion
- Milestone rewards at 7, 21, 30, 60 and 100 Perfect Days
- Persistent local data using IndexedDB
- JSON backup/restore
- Offline service worker after first hosted visit

## Mobile installation
For the service worker and installability, host these files on an HTTPS static site. Open that site in Chrome on Android, then use Chrome's menu → Add to Home screen / Install app.

No login is required by Pulse. Data is stored locally in the browser/site on the device. Export a backup periodically.

## Important
Do not open `index.html` directly from a downloaded ZIP and expect PWA/offline installation to work. Service workers require a secure context (normally HTTPS); `file://` pages are not suitable for this. Once hosted on HTTPS, refresh/reopen the site normally and then install it from Chrome.


## v3 date fix
Pulse now uses the phone's local calendar date for dates and daily records, preventing IST from displaying the previous UTC day.
