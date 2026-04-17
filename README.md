# TGF Weekly Review Dashboard · Talview

Executive dashboard for Thursday TGF calls. Pulls live data from Notion, shows 5 quarters of history, trend charts, and quarter comparison.

## Files

| File | Purpose |
|------|---------|
| `index.html` | Password login page |
| `dashboard.html` | Main dashboard |

## Changing the password

Open `index.html` and find this line near the top of the `<script>` block:

```js
const DASHBOARD_PASSWORD = 'Talview@TGF2026';
```

Change the value, commit, and push. The new password takes effect immediately.

## Updating the dashboard

Replace `dashboard.html` with the new version, then:

```bash
git add dashboard.html
git commit -m "Dashboard update"
git push
```

## Thursday workflow

- **1:05 PM IST** — Dashboard auto-fetches latest Notion page
- **1:30 PM IST** — Dashboard hard locks for the TGF call
- Auto-discovery finds this week's page by date in the page title

## Access

Deployed at: `https://YOUR_USERNAME.github.io/tgf-dashboard`

Share `index.html` URL with leadership. They enter the password once and stay logged in for 12 hours.
