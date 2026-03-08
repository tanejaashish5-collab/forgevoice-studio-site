# ForgeVoice Studio — AI Automation Agency

Production landing page for ForgeVoice Studio's workflow automation services.

## Stack

- **Architecture:** Single-file HTML with embedded CSS/JS — zero dependencies, zero build step
- **Hosting:** Vercel (static deployment)
- **Fonts:** Playfair Display, Plus Jakarta Sans, JetBrains Mono (Google Fonts)
- **Design:** Obsidian Precision v2 — pure black + warm gold accent

## Deploy

### Vercel CLI
```bash
vercel --prod
```

### GitHub Integration
Push to `main` branch → auto-deploys via Vercel GitHub integration.

### Custom Domain
1. Add domain in Vercel Dashboard → Project Settings → Domains
2. Update DNS records as instructed by Vercel
3. Update canonical URL and OG tags in `index.html` head

## Files

| File | Purpose |
|------|---------|
| `index.html` | Full landing page (HTML + CSS + JS) |
| `vercel.json` | Vercel config — security headers, caching, routing |
| `robots.txt` | Search engine crawl rules |
| `sitemap.xml` | SEO sitemap |
| `favicon.png` | Browser tab icon |
| `logo.png` | Brand logo |

## Custom Domain Checklist

When pointing a custom domain:
1. Update `<link rel="canonical">` in index.html
2. Update `<meta property="og:url">` in index.html
3. Update `<meta property="og:image">` URLs in index.html
4. Update `Sitemap:` URL in robots.txt
5. Update `<loc>` URL in sitemap.xml
