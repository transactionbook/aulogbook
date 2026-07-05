# Play Console → App content → Data safety form

The Data Safety form asks a series of questions. Here are the answers verbatim
for AuLogbook. Copy each into the matching Play Console field.

---

## Step 1: Does your app collect or share any of the required user data types?

**Answer: YES**

AuLogbook collects location, photos/videos, and "other user-generated content" (trip records, receipt data).

(It does NOT collect most of the categories Google asks about — see specifics below.)

---

## Step 2: Is all of the user data collected by your app encrypted in transit?

**Answer: NO** *(then click "N/A — the app does not transmit user data from the device")*

The app does not transmit user data off the device (except the Google Play Billing flow, which is fully encrypted by Google). The transit-encryption question does not apply.

---

## Step 3: Provide a way for users to request deletion of their data

**Answer: YES — and the mechanism is in-app**

Users can delete all data via Settings → Clear All Data. The Privacy Policy documents this. There is no server-side data to delete because data stays on the device.

---

## Step 4: Data types collected + processed

For EACH data type, answer:
- Collected? (Yes / No)
- Shared? (Yes / No)
- Processed ephemerally? (Yes / No)
- Required or optional?

### Personal info

| Data type | Collected? | Notes |
|---|---|---|
| Name | NO | |
| Email address | OPTIONAL | User can enter in Settings → Email Address to pre-fill exports. Stays on device. |
| User IDs | NO | No accounts |
| Address | NO | |
| Phone number | NO | |
| Race / ethnicity | NO | |
| Political / religious beliefs | NO | |
| Sexual orientation | NO | |
| Other personal info | NO | |

### Financial info

| Data type | Collected? | Notes |
|---|---|---|
| User payment info | NO | Google Play handles all payments; AuLogbook never sees card details |
| Purchase history | YES — Collected | Subscription status is read from Google Play. NOT shared. Used to determine Pro vs Free. |
| Credit score | NO | |
| Other financial info | NO | |

### Health and fitness

| Data type | Collected? |
|---|---|
| All | NO |

### Messages

| Data type | Collected? |
|---|---|
| All | NO |

### Photos and videos

| Data type | Collected? | Notes |
|---|---|---|
| Photos | OPTIONAL | User scans or imports receipt photos. Stored in app-private storage. NEVER transmitted. |
| Videos | NO | |

### Audio files

| Data type | Collected? |
|---|---|
| All | NO |

### Files and docs

| Data type | Collected? | Notes |
|---|---|---|
| Files and docs | OPTIONAL | Only when user imports a CSV file for Toll Sync. Processed on-device only. |

### Calendar

| Data type | Collected? |
|---|---|
| All | NO |

### Contacts

| Data type | Collected? |
|---|---|
| All | NO |

### Apps

| Data type | Collected? |
|---|---|
| Other apps installed | NO |
| App interaction / logs | NO — no analytics, no usage stats |

### Device or other IDs

| Data type | Collected? |
|---|---|
| Device or other IDs | NO |

### Location

| Data type | Collected? | Notes |
|---|---|---|
| Approximate location | NO | (We only collect precise location.) |
| Precise location | YES — Required | GPS tracking is the core function. Stays on device. NEVER shared. Used for trip distance + toll detection. |

### App activity

| Data type | Collected? | Notes |
|---|---|---|
| Search history | NO | |
| Browsing history | NO | |
| Installed apps | NO | |
| Other user-generated content | YES — Collected | Trip records + receipt records entered by the user. Stored on device. NOT shared. |
| Other actions | NO | |

### Web history

| Data type | Collected? |
|---|---|
| All | NO |

### App info and performance

| Data type | Collected? | Notes |
|---|---|---|
| Crash logs | YES — Collected | Stored locally in app-private storage (visible to the user via the Crash Logs screen). NEVER sent to developer. |
| Diagnostics | NO | |
| Other app performance data | NO | |

---

## Step 5: For each YES above — purposes

### Precise location
- **Purpose:** App functionality (this is the core feature)
- **Sub-purpose:** Accountable for tax / logbook record-keeping
- **Cannot change:** Yes (location is essential to the app's purpose)

### Photos
- **Purpose:** App functionality (receipt scanning)
- **Optional / required:** Optional (user can manually enter receipt data instead)

### Purchase history
- **Purpose:** App functionality (determining Pro vs Free tier)
- **Optional / required:** Required (no way to gate Pro features otherwise)

### Other user-generated content (trips + receipts)
- **Purpose:** App functionality (this is what the app does)
- **Optional / required:** Optional (user only enters what they want to track)

### Files and docs (CSV import)
- **Purpose:** App functionality (Toll Sync feature)
- **Optional / required:** Optional

### Crash logs
- **Purpose:** App functionality (in-app diagnostics screen)
- **Optional / required:** Required (always on, but only visible to the user; never transmitted)

---

## Step 6: Family apps / children

This app is NOT targeted at children. The Data Safety form for child-directed
apps does not apply. Answer the family-related questions accordingly.

---

## Important note about "Encryption in transit"

When Play Console asks "Is all of the user data collected by your app encrypted
in transit?", answer **NO** and then **select "N/A — the app does not transmit
user data from the device"** for each data type. This is the honest answer —
your app has no servers, so the question doesn't apply.

If you answer "YES" to encryption-in-transit when there is no transit at all,
Google may flag the inconsistency during review.
