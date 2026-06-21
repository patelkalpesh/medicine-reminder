# Medicine Reminder App v4.2

## Live URL
https://kalpeshpatel-mobilearts.github.io/medicine-reminder/

## Repo
https://github.com/KalpeshPatel-mobilearts/medicine-reminder

## Location
/mnt/c/Users/Dell/medicine-reminder/

## Contact
- Kalpesh Patel
- Phone/WhatsApp: +91 74058 56226
- Email: kal.shooter007@gmail.com
- Google Account: kal.shooter007@gmail.com

## Tech Stack
- Single-file PWA (index.html)
- Vanilla JS, no frameworks
- Google Drive appData sync (OAuth2 via GIS)
- Service Worker: network-first (sw.js)
- GitHub Pages hosting

## Google OAuth Client ID
157005612520-70t1peegtr1uoinrnjv2g9uk1geni5j8.apps.googleusercontent.com

## All Features (v4.2 - 28 features)
1. 🏠 Today - Schedule with Take/Snooze, next dose widget (hrs + min)
2. ✅ Auto-collapse taken doses
3. 💊 Medicines - Add/Edit/Pause, photo crop, SOS emergency
4. 📸 Photo upload with crop tool (drag + zoom)
5. ⏰ Reminders - 30/15/5/0 min configurable + sound alert
6. ⏰ Snooze - 10/30 min with countdown, syncs across devices
7. 📈 Weekly adherence % bar
8. 📅 Calendar - Monthly green/yellow/red view
9. 📝 Notes per dose (symptoms, BP readings)
10. ❤️ Health - BP log (upper/lower/heart rate) with history
11. 📅 Doctor appointments with countdown + reminders
12. 📦 Stock - Strips, balance, days left, stock-until date, timeline
13. 💰 Price per strip, cost calculator (15/30/60 days)
14. 🛒 Order Planner - What to buy for any period including current stock
15. ⚠️ Reorder alerts - configurable threshold (3-14 days), WhatsApp/Email/Notify
16. 🔁 Course duration - Day X/Y progress
17. 🏥 Doctors/Pharmacy - Contacts, tap-to-call, editable
18. 💬 Caretaker alerts - Auto WhatsApp if missed, editable
19. 🖨️ Print medicine card (fridge) - with Back button
20. 📊 Doctor report PDF - 30-day adherence + notes
21. 📄 Stock statement report - printable
22. 📋 History - Export WhatsApp/Email/PDF/Excel
23. 🔄 Backup/Restore - JSON file + WhatsApp share
24. ☁️ Google Drive sync - auto push/pull, syncs all data
25. 🔐 PIN lock - once per session
26. 🌙 Dark mode
27. 🌐 Languages - English/Hindi/Gujarati (tab names only currently)
28. 📲 Install - PWA with first-time install banner
29. 🆕 Auto update notifications
30. 📧 Monthly auto-email report
31. 📢 Share app button (WhatsApp + copy link)
32. ✨ About/Showcase page (collapsed)

## Data Storage
- localStorage keys: medicines2, med_logs2, med_doctors, med_caretakers, bp_logs, med_appointments, notif_settings, reorder_settings, snoozed, data_updated, gdrive_token, app_pin, dark_mode, app_lang, sound_on, report_email, reorder_days, reorder_alerted, install_banner_dismissed
- Google Drive: appDataFolder/medicine-reminder-data.json

## Default Settings
- WhatsApp: 917405856226
- Email: kal.shooter007@gmail.com
- Reorder threshold: 7 days
- PIN: user-set (first time)

## Tab Structure
🏠 Today | 💊 Meds | ❤️ Health | 📦 Stock | ⚙️ Settings

## PENDING (Next Session)
1. Hindi/Gujarati FULL translation (all labels, buttons, alerts - not just tabs)
2. Migrate repo to personal GitHub (kal.shooter007@gmail.com)
3. Google OAuth verification (remove "unverified" warning)
4. Privacy policy page (needed for Google verification)
5. Drug interaction warnings (optional)
6. Flexible schedules - Mon/Wed/Fri, alternate days, weekly (optional)

## Update/Deploy Process
1. Edit index.html
2. Update version.json
3. Update APP_VERSION const + version text in Settings
4. `git add -A && git commit -m "message" && git push origin main`
