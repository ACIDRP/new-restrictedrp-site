# Revolution Network — Netlify-ready frontend

This package has been prepared for Netlify static hosting.

## Deploy
- Set the Netlify publish directory to `public` (already configured in `netlify.toml`).
- Deploy the project root.
- `/`, `/events`, and `/staff/events` are configured as friendly routes.

## Important
The original project contains a Flask backend (`app.py`) with Discord OAuth,
sessions, an SQLite database, and server-side event APIs. Netlify static hosting
does not execute that Flask process.

This package therefore makes the existing frontend routable on Netlify, but
server-side Flask features still require a backend host or a migration to
Netlify Functions/serverless APIs.

The original Flask files and database are retained in the package.
