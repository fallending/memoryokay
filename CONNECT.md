# App Store Connect — values for Memoryo

Internal checklist only (not App Store metadata). Use after GitHub Pages is live.

## URLs

Confirm the GitHub username/org matches the live Pages host (default below uses `fallending`).

| Field | Where | Value |
|-------|--------|--------|
| **Privacy Policy URL** | App Privacy | `https://fallending.github.io/memoryokay/privacy.html` |
| **Support URL** | App version → each localization (English U.S., 简中, 繁中, 日本語, 한국어, Français, …) | `https://fallending.github.io/memoryokay/support.html` |

The same Support URL may be used for every language.

## App Information

| Field | Value |
|-------|--------|
| **Copyright** | `2026 Asusual` |
| **Content Rights** | Choose **No** — the app does not include third-party licensed media catalogs; it shows the user’s own Photos library and Asusual’s UI. (If you later embed licensed stock packs, revisit this.) |

## App Privacy questionnaire (Admin)

Typical answers for current Memoryo (local-first, no Asusual backend collection):

1. **Privacy Policy URL** → paste the URL above → Save.
2. **Data collection**: if you do **not** send user data to Asusual servers / analytics / ads SDKs → select that you **do not collect data** (or equivalent “No”), then publish.
3. Email feedback the user sends voluntarily is support correspondence, not App Store “data collection from the app” in the usual sense — keep product behavior aligned with `privacy.html`.
4. Click **Publish** / save so the privacy section is no longer blocking submission.

If you later add analytics, crash reporting, or accounts, update both the questionnaire and `privacy.html` before the next release.

## Enable GitHub Pages

1. Push this folder’s git repo to `git@github.com:fallending/memoryokay.git` (or your org’s equivalent).
2. GitHub → **Settings** → **Pages**
3. Source: **Deploy from a branch** → `main` → `/ (root)` → Save
4. Wait 1–2 minutes, open the Privacy & Support URLs in a browser, then paste into Connect
