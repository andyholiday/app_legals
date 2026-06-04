# App Legals

Legal pages (Privacy Policy, Support) for my iOS apps.

## Structure

```
app_legals/
├── metersnap/                    # Live legal pages
│   ├── index.html                → Redirect to privacy.html
│   ├── privacy.html              → Privacy Policy
│   └── support.html              → FAQ & Support
├── [future-app]/                 # Add more apps here
│   └── ...
└── _draft_jaszka_website/        # Draft: Full website for jaszka.com (Backlog)
    ├── index.html                → Homepage
    ├── apps/metersnap/           → App landing page
    └── legal/                    → Impressum, Datenschutz
```

## GitHub Pages URLs

**Live:**
- **MeterSnap Privacy:** `https://andyholiday.github.io/app_legals/metersnap/privacy.html`
- **MeterSnap Support:** `https://andyholiday.github.io/app_legals/metersnap/support.html`

**Draft (not deployed):**
- Full website prepared for jaszka.com hosting (Netcup)
- Located in `_draft_jaszka_website/`

## Adding a New App

1. Create folder: `[app-name]/`
2. Add `privacy.html` and `support.html`
3. Optional: `index.html` redirect
4. Commit and push

## Setup

1. Go to repository Settings → Pages
2. Source: Deploy from a branch
3. Branch: `main` / `root`
4. Save

## Vercel Deployment

This repo also deploys as a central static site on Vercel (`vercel.json` enables
clean URLs, so `.html` is optional). Used for the App Store Connect Privacy /
Support URLs.

- **MeterSnap Privacy:** `/metersnap/privacy`
- **MeterSnap Support:** `/metersnap/support`

Deploy: `vercel --prod` from the repo root.

---

© 2025 André Jaszka
