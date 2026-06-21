# Medicine Reminder App v3.2

## Live URL
https://kalpeshpatel-mobilearts.github.io/medicine-reminder/

## Repo
https://github.com/KalpeshPatel-mobilearts/medicine-reminder

## Tech Stack
- Single-file PWA (index.html)
- Vanilla JS, no frameworks
- Google Drive appData sync (OAuth2 via GIS)
- Service Worker: network-first (sw.js)
- GitHub Pages hosting

## Google OAuth Client ID
157005612520-70t1peegtr1uoinrnjv2g9uk1geni5j8.apps.googleusercontent.com

## Features (v3.2)
1. 🏠 Today - Schedule grouped by Morning/Afternoon/Evening with Take/Skip
2. ✅ Auto-collapse taken doses (expandable "X done" bar)
3. 💊 Medicines - Master list with photo, course info, stock
4. ➕ Add/Edit - Name, dosage, photo upload (camera/gallery), frequency (1x/2x/3x/SOS), timing per dose, time per dose, course duration, strip-based stock
5. 🆘 SOS Medicines - Emergency medicines with instructions and "Take Now" button
6. 📅 Calendar - Monthly view with green/yellow/red adherence dots
7. 📈 Weekly Adherence - % bar (taken/total over 7 days)
8. 📦 Stock Management - Strips × tablets per strip + loose, "Buy New Stock" button, auto-consume on Take, low stock alerts
9. 📷 Medicine Photos - Camera/gallery upload, compressed to 200px JPEG
10. 🔁 Course Duration - Day X/Y progress (7/14/21/30/60/90 days or ongoing)
11. 🏥 Doctor/Pharmacy - Add contacts with phone, specialty, next visit
12. 💬 Caretaker Alerts - Auto WhatsApp to family if dose missed by 30 min
13. 🔔 Notifications - Configurable 30/15/5/0 min before dose (2x2 grid UI)
14. ☁️ Google Drive Sync - Auto push on change, auto pull on load + visibility change, shows email + last sync time
15. 📲 Install App - One-click PWA install (Android native prompt, iOS instructions)
16. 🆕 Update Notifications - Blue banner when new version available, tap to refresh
17. 🔄 Refresh button at top
18. 📋 History - Date-wise log with export: WhatsApp, Email, PDF, Excel/CSV
19. ⚠️ Refill Alerts - On Today page when stock ≤5 (danger) or ≤1 strip (warning)

## Data Storage
- localStorage keys: medicines2, med_logs2, med_doctors, med_caretakers, notif_settings, data_updated, gdrive_token
- Google Drive: appDataFolder/medicine-reminder-data.json (syncs medicines, logs, doctors, caretakers)

## Tab Structure
🏠 Today | 💊 Meds | 📅 Calendar | 📦 Stock | ⚙️ Settings

## Update/Deploy Process
1. Edit index.html
2. Update version.json (version number + features text)
3. Update APP_VERSION const in index.html
4. Update version display text in Settings card
5. `git add -A && git commit -m "message" && git push origin main`
6. Users see blue "New version available" banner → tap to update

## iOS Notifications Setup
- Must install as PWA (Add to Home Screen with "Open as Web App" ✅)
- Requires iOS 16.4+
- Open from home screen icon (not Safari)

## Key Files
- `index.html` - The entire app (single file)
- `sw.js` - Service worker (network-first strategy)
- `manifest.json` - PWA manifest with maskable icons
- `version.json` - Version check for update notifications
- `icon.svg`, `icon-192.png`, `icon-512.png` - App icons
- `demo.html`, `demo-full.html` - Feature demos (can be deleted)
