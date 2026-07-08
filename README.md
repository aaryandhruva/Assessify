# Assessify — Marketing Site

Premium, single-page marketing experience for **Assessify** ("Smart Grading, Smarter Learning") — an AI grading engine for essays and open-ended assessments.

## What's inside
- `index.html` — the full site: hero, problem, platform, features, pipeline, competitive comparison, market, pricing, testimonials, FAQ, founder, investor CTA, contact.
- `vercel.json` — static hosting config with sensible caching + security headers.
- `robots.txt`, `sitemap.xml` — SEO essentials.
- `.env.example` — template for analytics + form endpoints.

## Design system
- **Display:** Space Grotesk · **Body:** Inter · **Data:** JetBrains Mono
- **Palette:** deep indigo `#4F46E5` → electric blue `#38BDF8` → purple `#8B7CF6`, near-black `#0A0A0B`, chartreuse accent `#C6E265`
- Dark mode by default with a full light theme toggle.

## Features
Sticky glass navbar · mobile menu · dark/light toggle · animated gradient blobs · scroll-reveal · animated counters · SVG score rings & donut charts · animated meters · live grading dashboard mockup · interactive comparison table · accordion FAQ · validated contact form · back-to-top · cookie consent · full responsive + reduced-motion support · WCAG-minded focus states, ARIA and semantic HTML.

No build step, no dependencies — everything is self-contained. Fonts load from Google Fonts.

## Run locally
Just open `index.html`, or serve it:
```bash
npx serve .
# or
python3 -m http.server 3000
```

## Deploy to Vercel
```bash
# 1) create the repo
git init && git add . && git commit -m "Assessify site"

# 2) push to GitHub (create the repo first at github.com/new)
git remote add origin https://github.com/<you>/assessify.git
git branch -M main
git push -u origin main

# 3) deploy — either import the repo at vercel.com/new,
#    or from the CLI:
npm i -g vercel
vercel            # preview
vercel --prod     # production
```
Vercel auto-detects this as a static site; no framework preset or build command needed.

## Notes on content
All copy is rewritten from the source pitch deck into original marketing language. Testimonials and partner logos are clearly labeled **illustrative placeholders**. Market and pricing figures reflect the deck; final pricing is set per institution.
