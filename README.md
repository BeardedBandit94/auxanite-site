# auxanite.com

Static website for Auxanite LLC. Plain HTML and CSS: no build step, no
JavaScript, no external requests.

| File | Purpose |
| --- | --- |
| `index.html` | Home: definition, apps list, about, contact |
| `support.html` | Use as the **Support URL** in App Store Connect |
| `privacy.html` | Use as the **Privacy Policy URL** in App Store Connect |
| `apps/template.html` | Copy for each app's own page |
| `404.html` | Not-found page (picked up automatically by most static hosts) |
| `styles.css` | All styling; colours are variables at the top |

## Adding an app

1. In `index.html`, find the `TO ADD AN APP` comment and follow it.
2. Copy `apps/template.html` to `apps/<your-app>.html` and fill it in.
3. Add the new page to `sitemap.xml`.

## Before going live

- The site links to `hello@auxanite.com` and `support@auxanite.com`. Create
  those mailboxes (or aliases), or search-and-replace the addresses.
- Read `privacy.html` and make sure every statement is true for your setup.
  If you add analytics or a contact form, update it.

## Deploying

Upload the folder as-is to any static host (Cloudflare Pages, Netlify,
GitHub Pages, Vercel) and point the `auxanite.com` DNS at it.
