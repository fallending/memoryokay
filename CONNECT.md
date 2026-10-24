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

Newer GitHub often only offers **GitHub Actions** (branch deploy may be missing). Prefer Actions:

1. Settings → **Pages** → **Build and deployment** → **Source** → **GitHub Actions**
2. Keep `.github/workflows/pages.yml` on `main` and push (or re-run under **Actions**)
3. When the workflow is green, open privacy/support URLs, then paste into Connect

If **Deploy from a branch** is available: `main` → `/ (root)` → Save.
