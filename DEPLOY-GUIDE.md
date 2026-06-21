# Medicine Reminder - Deployment & Verification Guide

## Live URLs
- **Primary (NEW):** https://patelkalpesh.github.io/medicine-reminder/
- **Old (keep for now):** https://kalpeshpatel-mobilearts.github.io/medicine-reminder/
- **Privacy Policy:** https://patelkalpesh.github.io/medicine-reminder/privacy.html

## Repos
- **Primary:** https://github.com/patelkalpesh/medicine-reminder
- **Old:** https://github.com/KalpeshPatel-mobilearts/medicine-reminder

## Push to patelkalpesh (from this PC)
```bash
cd /mnt/c/Users/Dell/medicine-reminder
git rm --cached .github/workflows/pages.yml
git commit -m "temp"
git push https://patelkalpesh:YOUR_PAT_TOKEN@github.com/patelkalpesh/medicine-reminder.git main
git add .github/workflows/pages.yml
git commit -m "re-add workflow"
git push origin main
```
PAT stored locally. Regenerate at https://github.com/settings/tokens

## Google OAuth Setup
- **Console:** https://console.cloud.google.com/apis/credentials
- **Client ID:** 157005612520-70t1peegtr1uoinrnjv2g9uk1geni5j8.apps.googleusercontent.com
- **Authorized JavaScript origins:**
  - https://patelkalpesh.github.io (NEW - added)
  - https://kalpeshpatel-mobilearts.github.io (OLD - remove later)

## Google Verification Steps (to remove "unverified" warning)
1. Go to: https://console.cloud.google.com/apis/credentials/consent
2. Fill in:
   - App name: Medicine Reminder
   - User support email: kal.shooter007@gmail.com
   - App logo: upload icon-192.png
   - App homepage: https://patelkalpesh.github.io/medicine-reminder/
   - Privacy policy: https://patelkalpesh.github.io/medicine-reminder/privacy.html
   - Terms of service: https://patelkalpesh.github.io/medicine-reminder/privacy.html
   - Authorized domains: patelkalpesh.github.io
3. Click "Submit for verification"
4. Wait 3-5 business days

## Until Verified (add test users)
1. Go to: https://console.cloud.google.com/apis/credentials/consent
2. Scroll to "Test users"
3. Add emails of people you share the app with (up to 100)
4. They can sign in without warning

## Remove Old URL (when ready)
1. Google Console → Credentials → OAuth Client → remove `https://kalpeshpatel-mobilearts.github.io` from origins
2. Delete repo: https://github.com/KalpeshPatel-mobilearts/medicine-reminder/settings → Danger Zone → Delete

## Accounts
- GitHub (primary): patelkalpesh
- GitHub (old): KalpeshPatel-mobilearts  
- Google (sync): kal.shooter007@gmail.com
- Google (console owner): kalpesh.patel@mobileartsme.com
- WhatsApp: 917405856226
- Email: kal.shooter007@gmail.com
