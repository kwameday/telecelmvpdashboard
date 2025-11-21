
# Telecel Marketplace Pilot — Payments & Cashback Dashboard (Static JSON)

This repo contains a static HTML dashboard that visualises Telecel Marketplace pilot performance.

It includes:

- Summary KPI cards (transactions, GMV, cashback, etc.)
- User metrics (total, unique, and repeat users)
- Cashback Leaderboard
- User Frequency Leaderboard (most active users)
- Daily Transaction Summary table

## Files

- `index.html` — Complete dashboard UI, styling, and rendering logic. It fetches `data.json`.
- `data.json` — All metrics, leaderboards, and daily breakdown.

## Deploy on Cloudflare Pages

1. Create a new GitHub repo (e.g. `telecel-dashboard`).
2. Add `index.html` and `data.json` to the root of the repo and commit.
3. In Cloudflare Dashboard → **Pages** → **Create a project** → **Connect to Git**.
4. Select your repo and set:
   - Framework preset: **None**
   - Build command: *(leave empty)*
   - Output directory: `/`
5. Deploy — your dashboard will be live at `https://<project>.pages.dev`.

## Updating Data

- Open `data.json` in GitHub and edit the numbers, leaderboard entries, or daily rows.
- Commit to `main` — Cloudflare Pages will redeploy automatically and the dashboard will update.
