# AC Repair Newtown Square PA — Astro Site

Static Astro site for **acrepairnewtownsquarepa.com**, optimized for Cloudflare Pages.

## Features
- Responsive, mobile-first design
- Cool blue + cyan color theme
- OpenStreetMap embed pinpointing 3728 West Chester Pike, Newtown Square, PA 19073
- SEO: meta tags, canonical, JSON-LD LocalBusiness schema, sitemap, robots.txt
- Blog section powered by Markdown content collections
- Fast static build for Google indexing
- Cloudflare Pages ready (static output, no adapter needed)

## Phone number
Placeholder: **(610) 555-0199** — replace across the site (search for `6105550199` and `555-0199`).

## Deploy to Cloudflare Pages
1. Push this folder to a GitHub/GitLab repo.
2. In Cloudflare Dashboard → Workers & Pages → Create → Connect to Git.
3. Build settings:
   - **Framework preset:** Astro
   - **Build command:** `npm run build`
   - **Build output directory:** `dist`
4. Add custom domain `acrepairnewtownsquarepa.com`.
5. Submit `https://acrepairnewtownsquarepa.com/sitemap-index.xml` in Google Search Console.

## Local development
```bash
npm install
npm run dev
```

## Build
```bash
npm run build
```
Output is in `dist/`.

## Notes
- Site is fully static (`output: 'static'` by default) — ideal for Pages and SEO.
- `@astrojs/sitemap` generates `/sitemap-index.xml` at build time.
- `public/robots.txt` points crawlers to the sitemap.
- Blog posts live in `src/content/blog/*.md`.
