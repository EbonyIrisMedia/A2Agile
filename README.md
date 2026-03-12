# A2Agile Inc. Website

Static HTML website for A2Agile Inc. — Agile training, coaching, and consulting based in Ann Arbor, MI.

## Deployment

**Stack:** Static HTML → GitHub (EbonyIrisMedia org) → Cloudflare Pages

### Setup Steps

1. Create repo `A2Agile` under `EbonyIrisMedia` GitHub org
2. Push this directory to the repo
3. In Cloudflare Dashboard → Pages → Create a project
4. Connect to the `EbonyIrisMedia/A2Agile` GitHub repo
5. Build settings:
   - **Framework preset:** None
   - **Build command:** (leave blank)
   - **Build output directory:** `/`
6. Deploy

### Custom Domain

After deployment, add custom domain `a2agile.com` (and `www.a2agile.com`) via Cloudflare Pages custom domains. Update DNS records as directed by Cloudflare.

## Structure

```
/
├── index.html    # Single-page site (self-contained HTML/CSS/JS)
└── README.md     # This file
```

## Features

- Fully responsive single-page design
- Schema.org structured data (ProfessionalService + FAQPage)
- Open Graph meta tags
- AEO-optimized FAQ schema
- Scroll-triggered animations
- Mobile navigation
- Contact form (client-side placeholder — connect to form service as needed)

## Notes

- Contact form currently uses a client-side placeholder. Connect to Cloudflare Workers, Formspree, or similar for production use.
- No external JS dependencies — pure vanilla HTML/CSS/JS.
- Google Fonts loaded: DM Serif Display + Outfit.
