# North Intelligence — northintelligence.se

Landing page for North Intelligence AB — independent data consultancy (Microsoft Fabric & Power BI), Stockholm. Static single-page site served via GitHub Pages. No build step: `index.html` is the whole site.

## Files

- `index.html` — the site (embedded CSS, no JavaScript, Google Fonts is the only external dependency)
- `favicon.svg` — the N-tile mark
- `CNAME` — custom domain for GitHub Pages
- `design/` — original Claude Design exports (design reference, not served)

## DNS setup for northintelligence.se

Add these records at your domain registrar:

| Type  | Host | Value                     |
|-------|------|---------------------------|
| A     | `@`  | `185.199.108.153`         |
| A     | `@`  | `185.199.109.153`         |
| A     | `@`  | `185.199.110.153`         |
| A     | `@`  | `185.199.111.153`         |
| CNAME | `www`| `simon-stenkoll.github.io`|

Once DNS has propagated (minutes up to ~24 h):

1. Go to the repo → **Settings → Pages** and confirm the custom domain `northintelligence.se` shows a green check.
2. Tick **Enforce HTTPS** (available once GitHub has issued the certificate).

Until then the site is live at https://simon-stenkoll.github.io/north-intelligence-website/

## Updating the site

Edit `index.html`, commit, push to `main`. GitHub Pages redeploys automatically within a minute or two.
