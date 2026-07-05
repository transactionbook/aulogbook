# Rideshare AuLogbook — Marketing site + Play Store listing assets

This folder contains everything needed to launch AuLogbook on the Google Play Store
and host a simple landing page. Hosted free via GitHub Pages.

## Folder contents

```
marketing/
├── index.html                 ← Landing page (hero + features + pricing + privacy band)
├── privacy-policy.md          ← Markdown Privacy Policy (also at ../privacy/PRIVACY_POLICY.md)
├── README.md                  ← This file
├── listing/
│   ├── play-store-listing.md  ← Title, short + full description, keywords for Play Console
│   ├── data-safety-form.md    ← Answers to the Data Safety form (Play Console → App content)
│   └── content-rating.md      ← IARC questionnaire answers
├── screenshots/               ← 8 Play Store screenshots (1080x1920 PNG)
│   ├── 01_track.png
│   ├── 02_receipts.png
│   ├── 03_verify.png
│   ├── 04_toll_sync.png
│   ├── 05_reports.png
│   ├── 06_dark_mode.png
│   ├── 07_multi_vehicle.png
│   └── 08_paywall.png
└── feature-graphic.png        ← 1024x500 banner for Play Store listing header
```

## Step-by-step: host the landing page (free, 10 minutes)

### Option A — GitHub Pages (recommended, fully free)

1. **Create a GitHub account** (if you don't have one) at github.com
2. **Create a new public repository** named `aulogbook` (or anything)
3. **Upload all files** from this `marketing/` folder to the repo root
4. **Enable GitHub Pages:**
   - Repo → Settings → Pages
   - Source: `Deploy from a branch`
   - Branch: `main` / `(root)`
   - Save
5. **Wait 1-2 minutes** — your site goes live at `https://<your-username>.github.io/aulogbook/`
6. **Use that URL** as your Privacy Policy URL in Play Console

### Option B — Netlify (drag-and-drop, also free)

1. Go to app.netlify.com/drop
2. Drag the entire `marketing/` folder onto the page
3. Get an instant URL like `https://aulogbook-xyz.netlify.app`
4. Optionally rename to a custom subdomain (free)

### Option C — Cloudflare Pages

1. Cloudflare dashboard → Pages → Create project
2. Connect the GitHub repo from Option A
3. Auto-deploys on every push

## Play Console — where each file goes

| Play Console field | Use this file |
|---|---|
| **App name** | `listing/play-store-listing.md` → "App name" |
| **Short description (80 chars)** | `listing/play-store-listing.md` → "Short description" |
| **Full description** | `listing/play-store-listing.md` → "Full description" |
| **App icon** | `C:\Users\TV\ZCodeProject\TripLog-RC\assets\icon.png` (1024x1024, already correct) |
| **Feature graphic** | `feature-graphic.png` (1024x500) |
| **Phone screenshots** | `screenshots/*.png` (upload 2-8 of them, in order) |
| **Privacy Policy URL** | Your GitHub Pages URL (from above) |
| **App content → Data safety** | Answers in `listing/data-safety-form.md` |
| **App content → Content rating** | Answers in `listing/content-rating.md` |

## Customising

- **Replace the email** `transactionbook@gmail.com` everywhere with your real support email
- **Replace the icon** `marketing/icon.png` (referenced by index.html) with the 1024x1024 master at `TripLog-RC/assets/icon.png`
- **Update the Play Store URL** in `index.html` once you know it (it'll be `play.google.com/store/apps/details?id=com.rideshare.aulogbook` — already pre-filled)

## Cost

$0. All hosting options listed are free for static sites.
