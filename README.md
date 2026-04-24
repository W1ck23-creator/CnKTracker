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


## v5.0.0
- Added minimal current streak and longest streak display to Tracker
- Added current streak and longest streak to Reports summary
- Uses forgiving streak logic:
  - a day counts with at least one entry
  - streak stays alive if the most recent logged day is today or yesterday


## v5.1.0
- Replaced plain Favorite Foods dropdown with a searchable autocomplete-style favorites field
- Type to filter favorites by any part of the food name
- Click or keyboard-select a favorite to autofill the entry form


## v5.2.0
- Added small Qty field to Tracker
- Qty defaults to 1 and allows decimals
- Macro values are multiplied by Qty when an entry is submitted
- Qty resets to 1 after saving an entry
