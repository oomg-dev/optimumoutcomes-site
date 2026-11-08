# optimumoutcomes-site

One-page site for Optimum Outcomes Management Group, served by GitHub Pages.

## Files
- `index.html` is the whole site. Text, layout, and styles live in this one file.
- `CNAME` (removed during review) tells GitHub Pages the custom domain. Add it back, containing `www.optimumoutcomes.com`, right before the DNS cutover. While it exists, the github.io preview address redirects to the custom domain.
- `.nojekyll` tells GitHub to serve the files as-is.

## Turn on Pages
Settings > Pages > Build and deployment > Source: Deploy from a branch > Branch: main, folder: / (root) > Save.
After DNS is set, check "Enforce HTTPS" on the same screen.

## DNS at GoDaddy
Change only these. Leave the Zoho MX and TXT records alone.

| Type  | Name | Value                |
|-------|------|----------------------|
| A     | @    | 185.199.108.153      |
| A     | @    | 185.199.109.153      |
| A     | @    | 185.199.110.153      |
| A     | @    | 185.199.111.153      |
| CNAME | www  | oomg-dev.github.io   |

Delete any existing A record for @ or CNAME for www that points to GoDaddy's site builder first.

## Editing
Change text in `index.html`, commit to main, and the site updates in a minute or two.
