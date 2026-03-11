# TubeMind – Privacy Policy

*Last updated: March 2024*

## Overview
TubeMind is a Chrome extension that helps you organize YouTube videos. 
We are committed to protecting your privacy.

## Data Storage
All your data (saved videos, categories, notes, settings) is stored 
**locally in your browser** using Chrome's built-in storage API. 
We do not have access to this data. It never leaves your device.

## Premium License
If you purchase TubeMind Premium, we collect only:
- Your email address (to deliver your license key)
- Your name (from payment processor)
- Country (from payment processor)

This data is stored securely and never sold or shared with third parties.
It is used solely to deliver and support your license.

## Permissions We Use
- **storage** – Save your video library locally in Chrome
- **activeTab** – Detect YouTube pages to show Save buttons
- **scripting** – Inject Save buttons onto YouTube thumbnails  
- **alarms** – Schedule your daily Watch Today reminders
- **notifications** – Show reminder notifications
- **host_permissions (youtube.com)** – Required to interact with YouTube pages

## Third Parties
TubeMind does not use any analytics, advertising, or tracking services.

## Children's Privacy
TubeMind is not directed at children under 13.

## Changes
We may update this policy. Continued use after changes means acceptance.

## Contact
Questions? Email: **anmolmishra51032@gmail.com**
```

**Step 4** — Commit the changes (click "Commit changes" green button)

**Step 5** — Go to repository **Settings** → scroll to **"Pages"** section → under Source select **"Deploy from branch"** → Branch: `main` → Click **Save**

**Step 6** — Wait 2 minutes → your privacy policy is live at:
```
https://yourusername.github.io/tubemind-privacy
```

That's your privacy policy URL. Done.

---

## Your Folder Structure — One Problem

Looking at your screenshot, your structure is:
```
TubeMind – YouTube Video Organizer/
├── icons/
├── popup/
├── background.js
├── content.css
├── content.js
└── manifest.json        ✅ correct
```

This is correct **BUT** your folder name has a problem:

> ❌ `TubeMind – YouTube Video Organizer` — the **em dash (–) and spaces** in the folder name can cause issues when zipping on Windows.

**Fix it** — rename the folder to simply:
```
tubemind
```

Then zip it correctly on Windows:
- Open the `tubemind` folder
- Select **all files inside** (Ctrl+A)
- Right click → **"Compress to ZIP file"** (Windows 11) or **Send to → Compressed folder**
- Do NOT zip the folder itself — zip the **contents**

The zip should extract directly to these files, not to a subfolder:
```
icons/
popup/
background.js
content.css
content.js
manifest.json
