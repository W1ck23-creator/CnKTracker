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

## Current Stable Version
v4.0.1

## In Progress
feature/favorites-and-polish

### Planned for v4.1.0
- [ ] Save favorite food option
- [ ] Daily total colors turn green when goal is met
- [ ] Remove "Synced with Supabase..." message
