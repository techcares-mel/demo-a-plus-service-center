# CLAUDE.md — A Plus Service Centre

## Business Details
- **Name**: A Plus Service Centre
- **Type**: Mechanic / Automotive Service Centre
- **Address**: 43 Market Rd, Sunshine VIC 3020, Australia
- **Phone**: 0447 345 261 | (03) 9366 0920
- **Email**: aplusservicecenter43@gmail.com
- **Website**: https://aplusservicecentre.com.au/ (currently unreachable)
- **Social**: Facebook: https://www.facebook.com/aplusservicecenter | Instagram: https://www.instagram.com/aplu_s16/

## Language
- ALL site text in English only. Brand name "A Plus Service Centre" used exactly as stated.

## Design System
- **Theme**: Dark (dark background, amber/gold accent)
- **Template**: A — Auto / Trades / Industrial
- **Accent color**: #ec9434 (orange/amber, extracted from images/logo.jpg)
- **Accent hover**: #efa452
- **Accent glow**: rgba(236, 148, 52, 0.25)
- **Background**: #0a0a0a
- **Surface**: #1a1a1a
- **Card**: #242424
- **Text**: #ffffff
- **Text muted**: #a0a0a0
- **Border**: rgba(255,255,255,0.08)
- **Heading font**: Oswald (700 headings, 500 nav/buttons)
- **Body font**: Roboto (400 regular, 500 emphasis)
- **Inspiration**: Dark industrial automotive aesthetic. Near-black backgrounds, amber/gold accents, bold condensed Oswald headings. Full-bleed hero with darkened photo overlay. Section alternation between #0d0d0d and #1a1a1a.

## Assets
- **Logo**: images/logo.jpg — user-provided. Referenced in nav (height: 48px) and footer (height: 56px).
- **images/**: user-provided photos. Place files as `image1.jpg`, `image2.jpg`, etc.
  - image1.jpg — used as hero background
  - image2.jpg — used as About section image (with "Sunshine, VIC" badge overlay)
  - image3.jpg–image6.jpg — gallery images
  - Add or replace any image file; the gallery automatically uses all images found in this folder.

## Page Sections (in order)
1. **Nav** — Fixed top, transparent on load, blurs on scroll >50px. Logo left, nav links right, hamburger below 768px.
2. **Hero** (#home) — Full-bleed image1.jpg with 62% dark overlay. Business name h1 with amber "SERVICE" em. Tagline, two CTAs (Book a Service / Call Us Now), trust strip (15+ years, 5-star reviews, all makes, same-day).
3. **Why Choose Us** (#why) — Surface bg. 4-card grid: Certified Mechanics, Transparent Pricing, All Makes & Models, Fast Turnaround. Icon circles with amber glow.
4. **Services** (#services) — Dark bg. 11 service cards in 3-col grid, each with icon block + description. All real services from research.json.
5. **Stats** (#stats) — Surface bg. 4 stats: 31+ Reviews, 5★ Rating, 15+ Years, 100% Honest Diagnostics. Count-up animation.
6. **Gallery** (#gallery) — Dark bg. 6 images in CSS grid (first item spans 2col×2row). Hover caption overlay.
7. **About** (#about) — Surface bg. 2-col: left = description + feature list; right = image2.jpg with "Sunshine, VIC" badge.
8. **Testimonials** (#testimonials) — Dark bg. 3 real Google reviews from research.json. 5-star rated.
9. **Contact** (#contact) — Dark bg. Left: phone (both numbers), email, address, trading hours (Mon–Fri 8AM–7PM, Sun 9AM–7PM), Google Maps embed. Right: contact form.
10. **Footer** — #0a0a0a bg. 4-col: brand + social icons (Facebook, Instagram), quick links, top 4 services, contact info.

## Rules
- Mobile-first, breakpoints: 480/768/1024/1280px
- Scroll-reveal on all cards and headings (80ms stagger via .d1/.d2/.d3/.d4 delay classes)
- Back-to-top button (fixed bottom-right, visible when scrollY > 300)
- DEMO watermark (fixed right side, rotated 90deg, opacity 0.09, amber color)
- Scroll progress bar (fixed top, 3px, amber)
- No Lorem Ipsum — real business data only
- Pure HTML5/CSS3/vanilla JS — no frameworks, no build step
- Font Awesome 6.5.0 CDN included (Facebook + Instagram social links present)

## Redeployment
After making changes, commit and redeploy from inside this folder:
```bash
git add -A
git commit -m "describe your changes"
git push
vercel --prod --yes
```
The Vercel project is already linked (`.vercel/project.json`) — no token or scope flags needed.
