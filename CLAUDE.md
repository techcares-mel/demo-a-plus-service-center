# CLAUDE.md — A Plus Service Centre

## Business Details
- **Name**: A Plus Service Centre
- **Type**: Automotive mechanic / car service centre
- **Address**: 43 Market Rd, Sunshine VIC 3020, Australia
- **Phone**: 0447 345 261 / (03) 9366 0920
- **Email**: aplusservicecenter43@gmail.com
- **Website**: https://aplusservicecentre.com.au/ (currently unreachable)
- **Facebook**: https://www.facebook.com/aplusservicecenter
- **Instagram**: https://www.instagram.com/aplu_s16/
- **Google Rating**: 5.0 stars, 31 reviews
- **Key Staff**: Sam (lead mechanic)

## Design System
- **Theme**: Dark
- **Primary color**: #e8a020 (amber — extracted from logo via colors.json)
- **Accent color**: #e8a020 (amber)
- **Accent hover**: #f5b835
- **Accent glow**: rgba(232, 160, 32, 0.25)
- **Background**: #0d0d0d
- **Surface**: #1a1a1a
- **Card**: #242424
- **Text**: #ffffff
- **Text muted**: #a0a0a0
- **Border**: rgba(255,255,255,0.08)
- **Heading font**: Syne (700, 800)
- **Body font**: Inter (400, 500, 600)
- **Inspiration**: Modern automotive service site, inspired by repairphones.com.au layout — service-focused, trust-building, dark amber theme. Balances professional credibility with approachable consumer-facing messaging.

## Page Sections
1. **Nav** — Fixed top. Logo + brand name left, links right. Blur on scroll. Hamburger below 1024px.
2. **Hero** — 100vh. Background image (image1.jpg) with dark overlay. h1, tagline, 4 trust badges, 2 CTAs.
3. **Why Choose Us** — 4-column icon strip: Expert Mechanics, Transparent Pricing, Fast Service, All Makes & Models.
4. **Services** — 11 service cards in 3-column grid (from research.json services[]).
5. **Stats** — 4 count-up counters: 31+ reviews, 5★ rating, 15+ years experience, 100% honest diagnostics.
6. **Gallery** — 5 images in CSS grid with hover zoom. First image spans 2 columns.
7. **About** — Two-column: text about Sam + community focus (left), image2.jpg (right) with badge overlay.
8. **Testimonials** — 3 review cards with stars, quotes, and author info (from research.json testimonials[]).
9. **Contact** — Address, 2 phones, email, trading hours, Google Maps embed, contact form with success state.
10. **Footer** — Logo, tagline, social icons (Facebook + Instagram only), links, contact info, copyright 2025.

## Rules
- Mobile-first, breakpoints: 480px / 768px / 1024px / 1280px
- Scroll-reveal animations on all cards and headings (fade + slide-up, 80ms stagger via .d1–.d4 classes)
- Back-to-top button (fixed bottom-right, appears at 300px scroll)
- DEMO watermark (position: fixed right side, rotated 90deg, opacity 0.09, font-size 100px)
- Scroll progress bar (position: fixed top, height 3px, amber accent color)
- Stats count-up via requestAnimationFrame over 1.5s with easeOutQuad
- Active nav link tracking via IntersectionObserver
- No Lorem Ipsum — all content from research.json
- Pure HTML5 / CSS3 / Vanilla JS — no frameworks, no build step
- Font Awesome 6.5.0 via CDN (used for social icons and UI icons)
- Google Fonts: Syne + Inter via CDN
