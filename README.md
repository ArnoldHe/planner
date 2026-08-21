# Planner

A single-page calendar + task planner that syncs with Google Calendar. Installable to an iPhone/Android home screen (PWA).

## Files
- `index.html` — the whole app (HTML, CSS, JS in one file)
- `manifest.json` — makes it installable as an app
- `icon.png`, `icon-512.png` — home-screen icons

## Modes
- **Quick add** — no setup; typed events open in Google Calendar to Save.
- **Full sync** — two-way sync via the Google Calendar API. Needs an OAuth Client ID.

## Setup for Full sync
The OAuth **Client ID** is set in `index.html` (`GOOGLE_CLIENT_ID`). It is public and safe to commit.
The OAuth **client secret** is NOT used by this app and must never be committed or deployed.

Authorized JavaScript origin for the Client ID must match the deployed site URL
(e.g. `https://christineplanner.netlify.app`).

## Deploy
Hosted on Netlify. Pushing to the connected branch auto-deploys.
