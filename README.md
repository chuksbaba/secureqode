# SecureQode Website

Value-added cybersecurity distributor for Africa. Static HTML/CSS/JS site.

## Structure

```
secureqode/
├── index.html          Homepage
├── solutions.html      Digital City 360° Shield — six pillars
├── services.html       VAD services model
├── vendors.html        Vendor portfolio + call for vendors
├── partners.html       Partner benefits
├── resources.html      Resources hub (placeholder)
├── about.html          Company narrative
├── contact.html        Contact page
├── css/styles.css      Design system
└── js/main.js          Mobile nav + minor interactions
```

## Deployment

### Option 1 — Netlify (recommended, free)
1. Push this folder to a GitHub repo
2. Go to [netlify.com](https://netlify.com) → New site from Git → select repo
3. Build command: leave blank. Publish directory: `/` (or root)
4. Deploy

### Option 2 — Vercel
1. Push to GitHub
2. [vercel.com](https://vercel.com) → Import Project
3. Framework preset: **Other**. Build command: blank. Output: `.`
4. Deploy

### Option 3 — GitHub Pages
1. Push to GitHub
2. Repo Settings → Pages → Source: `main` branch, `/` root
3. Site publishes at `https://yourusername.github.io/repo-name/`

### Option 4 — Any shared host / cPanel
Upload the entire folder contents to `public_html/` via FTP or the file manager.

## Custom Domain

Point your domain (e.g., `secureqode.com`) at your host:

- **Netlify/Vercel:** Add custom domain in dashboard → update DNS at your registrar per their instructions
- **GitHub Pages:** Add `CNAME` file with your domain, configure DNS A/CNAME records
- **cPanel:** Add domain as an addon domain, point DNS to host's nameservers

## Editing Content

- **Copy:** Edit the HTML files directly. All text is inline — no CMS.
- **Contact email:** Search for `hello@secureqode.com` and replace if needed.
- **Colors / branding:** Edit CSS variables in `css/styles.css` under `:root`.
- **Add a resource/blog post:** Copy a `.resource-card` block in `resources.html` and update text.

## What's Not Included

- No contact form (contact is by email per the brief)
- No analytics (add Google Analytics / Plausible / Fathom before launch if desired)
- No cookie banner (add if you serve EU/UK visitors or use tracking)
- No vendor logos (portfolio is category-based per the brief)

## Pre-Launch Checklist

- [ ] Confirm `hello@secureqode.com` is live and monitored
- [ ] Replace `[EDIT: ...]` placeholder text in `about.html`
- [ ] Add a favicon (`favicon.ico` in root, link in `<head>`)
- [ ] Add Open Graph meta tags if you want rich link previews
- [ ] Decide on analytics provider and add tracking snippet
- [ ] Test on mobile (Chrome DevTools device mode)
- [ ] Run Lighthouse audit for performance/SEO
