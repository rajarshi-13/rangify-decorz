# Rangify Decorz — Premium Event Management Website

## Overview
Complete premium website for Rangify Decorz, the leading event management company in Unnao, Kanpur & Lucknow. Built with pure HTML, CSS, and JavaScript — no framework dependencies.

---

## File Structure

```
rangify-decorz/
├── index.html              ← Homepage (main landing page)
├── sitemap.xml             ← SEO sitemap
├── css/
│   └── style.css           ← All styles (Black & Gold luxury theme)
├── js/
│   └── main.js             ← All JavaScript (animations, FAQ, forms)
├── images/                 ← Add your event photos here
└── pages/
    ├── about.html          ← About Us page
    ├── services.html       ← Full services breakdown
    ├── upcoming-events.html← Grand Launch + countdown
    ├── portfolio.html      ← Events gallery with filters
    ├── sponsorship.html    ← Sponsorship & partnership tiers
    ├── contact.html        ← Contact form + city info
    └── book.html           ← Booking form (conversion page)
```

---

## Pages Included

| Page | Purpose |
|------|---------|
| `index.html` | Hero, services, how-it-works, testimonials, FAQs, CTA |
| `about.html` | Story, values, team, timeline |
| `services.html` | All 8 service categories with full detail |
| `upcoming-events.html` | Grand Launch with live countdown + register form |
| `portfolio.html` | Filterable event gallery |
| `sponsorship.html` | 3-tier sponsorship + partner inquiry form |
| `contact.html` | Contact info + message form |
| `book.html` | Full booking form — highest-converting page |

---

## Quick Setup

1. **Open locally** — just open `index.html` in any browser. No server required.
2. **Update phone numbers** — search & replace `+919876543210` across all files with your actual number.
3. **Update email** — replace `hello@rangifydecorz.com` with your email.
4. **Add images** — place event photos in the `/images/` folder and update `background` or `src` attributes in HTML where placeholder divs exist.
5. **Update event date** — in `upcoming-events.html`, find the `targetDate` in the `<script>` block and set your actual launch date: `const targetDate = new Date('2025-MM-DDTHH:MM:SS');`
6. **Update team names** — in `about.html`, replace "Founder Name", "Event Lead Name", etc.
7. **Connect forms** — integrate with Formspree, Netlify Forms, or your backend for form submissions.

---

## Customization

### Colors (css/style.css — top of file)
```css
--gold: #c9a84c;          /* Main gold */
--gold-light: #e8c96e;    /* Lighter gold */
--black: #0a0a0a;         /* Background */
--black-card: #161616;    /* Card background */
```

### Fonts
Currently using Google Fonts:
- **Playfair Display** — headings/display
- **Cormorant Garamond** — subheadings, quotes
- **Montserrat** — body text, labels

### Adding Real Event Photos
Replace placeholder `<div class="portfolio-card-img">` elements with actual `<img>` tags:
```html
<img src="../images/wedding-01.jpg" alt="Royal Wedding Kanpur" style="width:100%;height:100%;object-fit:cover;" />
```

---

## SEO Setup

- All pages have `<title>`, `<meta name="description">`, and `<meta name="keywords">` tags
- Local SEO keywords: Unnao, Kanpur, Lucknow event management
- `sitemap.xml` included — submit to Google Search Console
- Update `<link rel="canonical">` in `index.html` to your actual domain
- Add your actual domain to all `og:` tags

---

## Conversion Features Included

- ✅ Sticky side CTA buttons (Book Event / Call Now)
- ✅ Floating WhatsApp button (animated)
- ✅ Multiple CTAs per page
- ✅ Lead capture forms on every page
- ✅ Counter animations (stats)
- ✅ Scroll-triggered fade animations
- ✅ FAQ accordion
- ✅ Mobile-responsive hamburger menu
- ✅ Countdown timer (upcoming events)
- ✅ Form validation with success feedback
- ✅ Portfolio image hover effects

---

## Deployment

### Option 1: Static Hosting (Recommended)
- **Netlify** — drag & drop the `rangify/` folder at netlify.com/drop
- **Vercel** — `vercel deploy` in the project root
- **GitHub Pages** — push to GitHub, enable Pages in settings

### Option 2: cPanel Hosting
Upload all files via cPanel File Manager to `public_html/`

---

## Form Integration (Production)

To make forms actually send emails, add Formspree:
1. Sign up at formspree.io
2. Create a form and get your endpoint (e.g. `https://formspree.io/f/yourcode`)
3. In each `<form>` tag, add: `action="https://formspree.io/f/yourcode" method="POST"`
4. Remove the fake success simulation in `main.js`

---

## Credits
Designed for Rangify Decorz — Premium Event Management
Unnao | Kanpur | Lucknow | Uttar Pradesh

Design: Black & Gold Luxury Theme
Fonts: Google Fonts (Playfair Display, Cormorant Garamond, Montserrat)
Icons: Unicode Emoji
