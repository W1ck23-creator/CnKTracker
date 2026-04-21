# CnKTracker v4.0 (Supabase-backed)

This version switches the tracker from local-only browser storage to Supabase-backed syncing.

## Files
- `index.html` = synced tracker
- `reports.html` = synced reports
- `config.js` = Supabase URL + publishable key
- `README.md` = setup notes

## Important before upload
Open `config.js` and replace:

`PASTE_YOUR_SUPABASE_PUBLISHABLE_KEY_HERE`

with your real Supabase publishable key.

The Project URL is already filled in.

## App flow
- One household login
- Two profiles inside the app: Chat and Kit
- The app remembers the last profile used on each device/browser

## What this version syncs
- daily entries
- goals
- tracking options
- reports

## Upload to GitHub Pages
Upload these files to the repo root:
- `index.html`
- `reports.html`
- `config.js`

Then commit and wait for Pages to republish.


## v4.1.0 (partial)
- Removed the synced-with-Supabase tracker message
- Daily total values stay black until goal is met, then turn green
