# Rideshare AuLogbook — Privacy Policy

**Last updated:** 5 July 2026
**Package:** `com.rideshare.aulogbook`
**Contact:** transactionbook@gmail.com  *(replace with your real email)*

This Privacy Policy describes how Rideshare AuLogbook ("AuLogbook", "we", "the app") handles your information when you use the app on your Android device.

## Summary (TL;DR)

**AuLogbook does not collect, transmit, sell, or share your personal data.** Everything the app records stays on your phone. We have no servers. We do not run analytics. We do not show ads. We do not have user accounts.

The app uses your phone's GPS, camera, and photo library — but only to perform its core functions (trip tracking and receipt scanning), and the data from those stays in app-private storage that other apps cannot read.

## 1. Information the app collects

### 1.1 Location data (GPS)
- **What:** Continuous GPS coordinates while a shift is active, plus intermittent location samples while the autostart monitor is armed.
- **Why:** To record trip distance for tax logbook purposes (ATO logbook method) and to detect toll-road crossings.
- **Where it goes:** Stays on your device. Stored in Android's app-private storage. **Never transmitted off the device.**
- **Foreground vs background:** Location is captured both while the app is open and while it is in the background (so tracking continues when you switch to Uber/Didi). This is essential to the app's core function — without it, trip distances would be inaccurate and your tax logbook invalid.

### 1.2 Camera + photo library access
- **What:** Camera access for scanning fuel/service receipts; photo library access for importing existing receipt photos.
- **Why:** To capture and smart receipt scanning for BAS / tax deduction records.
- **Where it goes:** Receipt images are stored in Android's app-private storage. Saving a copy to your phone's photo album is **opt-in per receipt** (a separate action you must take; never automatic).

### 1.3 Receipt + trip data
- **What:** Trip records (start/end time, distance, route summary, tolls, vehicle used) and receipt records (date, merchant, amount, GST, litres, ABN, scan confidence).
- **Why:** These are the records the app exists to produce — your tax logbook.
- **Where it goes:** Stays on your device in app-private storage. **Never transmitted off the device.**

### 1.4 Subscription status
- **What:** Whether you have an active Pro subscription (Google Play subscription ID + purchase state).
- **Why:** To unlock Pro features (unlimited receipts, XLSX export, Toll Sync, multi-vehicle).
- **Where it goes:** Subscription validation is handled by Google Play Billing. The app reads your purchase status from Google Play on the device; we never see your payment details.

## 2. Information the app does NOT collect

AuLogbook does **not** collect, store, or transmit:

- Your name, email, phone number, or address (unless you voluntarily enter your email in Settings for export pre-fill — and even then it stays on-device)
- Your Uber or Didi account credentials, fares, or trip data
- Your bank or credit card details
- Your E-Toll account credentials (Toll Sync uses the official CSV export that **you** download from your own browser — the app never sees your E-Toll login)
- Analytics data, usage statistics, or crash logs sent to a server
- Advertising identifiers (we do not run ads)
- Diagnostic data sent to third parties

## 3. Background location justification

AuLogbook uses background location because it is essential to the app's core function: recording an accurate logbook for tax purposes. Rideshare drivers switch between AuLogbook and Uber/Didi throughout a shift. If location tracking stopped when the app went to background, every shift would be incorrectly recorded — making the logbook invalid for the ATO.

We use Android's Foreground Service (with a persistent notification) for active shifts, and the autostart monitor (a lower-power background task) for detecting when a shift starts.

Background location is **never used for advertising, analytics, or any purpose other than recording your own trips**.

## 4. Data sharing

AuLogbook does **not** share data with any third party. We have no servers, no analytics, no advertising SDKs.

The only data that leaves your device is:

1. **When you explicitly export** (CSV, XLSX, PDF, JSON backup): the file goes to wherever you choose to save or share it (your email, cloud drive, etc.). This is a user-initiated action — the app does not auto-export.
2. **When you subscribe to Pro**: Google Play processes the payment; we receive only the subscription status (active/inactive), never your payment details.

## 5. Data retention + deletion

- Data is retained on your device until you delete it.
- You can delete individual trips and receipts via the in-app UI.
- You can delete **all** data via Settings → Clear All Data.
- Uninstalling the app deletes all data (Android wipes app-private storage on uninstall). The optional SAF backup folder (if you configured one) is the only data that survives uninstall — and that's stored in a folder you chose, controlled by you.

## 6. Children's privacy

AuLogbook is not directed at children under 13 (or the applicable age in your country). The app is a business tool for adult rideshare drivers. We do not knowingly collect data from children.

## 7. Your rights

Because we do not collect or store your data on our servers, you already have full control:

- **Access:** All your data is in the app, viewable at any time.
- **Export:** Use Settings → Export to CSV / XLSX / PDF / JSON backup.
- **Delete:** Use Settings → Clear All Data, or uninstall the app.

If you have a question about your data, contact us at the email above.

## 8. Security

- All data is stored in Android's app-private storage, sandboxed from other apps.
- The app does not transmit data over the network (except Google Play Billing for subscriptions).
- We do not store any passwords, tokens, or credentials.

## 9. International transfers

Because the app does not transmit your data anywhere, there are no international data transfers. Your data stays on your device.

## 10. Changes to this policy

If we change this Privacy Policy, we will update the date at the top of this page and notify users via the app's release notes. Continued use of the app after changes constitutes acceptance.

## 11. Implementation details

AuLogbook is built using industry-standard mobile development frameworks. All receipt
scanning and smart detection runs **entirely on your device** — no images or extracted
text are ever transmitted to any server. Specific libraries and frameworks used are
proprietary implementation details and are not disclosed publicly.

---

**Questions?** Contact: transactionbook@gmail.com  *(replace with your real email)*
