# Stay #1 — Aji Fruit Farm

**Owner:** Ajith (Aji)
**Location:** Embilipitiya, Sabaragamuwa Province, Sri Lanka
**Live site:** [aji-fruit-farm.lk](https://aji-fruit-farm.lk)
**Repo:** [yfelig/ajis-mango-farm](https://github.com/yfelig/ajis-mango-farm)
**Domain:** `aji-fruit-farm.lk` — purchased via Register.lk, DNS pointed to GitHub Pages
**Built:** May 2026

---

## The Property

Fifteen acres of tropical fruit orchard (mango, banana, rambutan, dragon fruit, coconut) beside a lake in rural Sri Lanka. Aji farmed commercially for 20 years — by 2018 ranked Sri Lanka's top commercial fruit farm. The 2020 pandemic and 2021 fertilizer ban forced a pivot. He built four private lakeside cottages in the orchard, each with polished concrete floors, a handmade teak bed, and an open-air bathroom with no roof.

Not a resort. Cold showers. Nature is very close. Kayaks on the lake. Udawalawe elephant safari 45 minutes south.

WhatsApp: `+94 70 506 5061`

---

## What Was Built

A 4-page static site (HTML/CSS/vanilla JS) hosted on GitHub Pages with a custom `.lk` domain:

| Page | URL | Purpose |
|------|-----|---------|
| Homepage | `/` | Full story: welcome, host intro, rooms teaser, setting, activities, food, reviews, contact |
| The Room | `/rooms.html` | 12-photo slider, room specs, amenities list, book CTA |
| The Farm | `/farm.html` | Setting, photo grids, lake section, activities, food carousel, book CTA |
| Our Story | `/story.html` | 3-act narrative: Six Years Away → Number One → Everything Changed |

**Photo count:** 26 real photos from Rivka's shoot placed across all pages. 6 food photos in horizontal scroll carousel. 12 room photos in slider.

---

## Design Decisions

- **Color:** Warm linen `#f0ede4` background + deep forest green `#1b3826` for CTAs. Matched the tropical farm environment.
- **Fonts:** Cormorant Garamond (display) + Inter (body). Boutique editorial feel — unusual for Sri Lanka guesthouses, which all use generic templates.
- **Primary CTA:** WhatsApp everywhere — floating button, nav button, dark footer on every page. Pre-filled booking message. No Airbnb link.
- **Reviews:** 6 real quotes from Airbnb + TripAdvisor, rotating carousel with amber gold stars (`#c8952e`).
- **Honest note:** "This is a working fruit farm in rural Sri Lanka — showers are cold water, and the nature is close. Not a five-star resort." On the rooms page. Trust-builder.
- **4-page model:** Richer than a single-page site. Each page tells a complete story. Story page especially strong — 3-act narrative drives emotional connection.

---

## Key Lessons

- The story page was the best decision. Aji's history (abroad → farming → crisis → cottages) is genuinely compelling. It converts browsers into bookers.
- Never use close-up abstract shots (door handles, fabric texture) as teaser photos on the homepage. Every grid image must answer: *what does this look like?*
- Cold showers are honest — put the disclaimer on the rooms page. It pre-qualifies and builds trust.
- Pre-filled WhatsApp message matters. One tap to inquire.
- Country-code domains (`.lk`) are cheap and give local credibility.

---

## Collaborators

- **Yair** — built the site (HTML/CSS/JS, GitHub Pages, DNS)
- **Rivka** — photographer (46 photos submitted; 26 placed, 39 extras in `/photos/`)
- **Aji** — owner, reviewed the site and approved copy
- Rivka added as GitHub collaborator (`rivsh4-a11y`) with push access

## Files

```
ajis-mango-farm/
├── index.html          ← Homepage
├── rooms.html          ← The accommodation
├── farm.html           ← The setting
├── story.html          ← Aji's story
├── style.css           ← Shared styles
├── script.js           ← Reviews carousel + nav scroll
├── photos/             ← 26 real photos (JPG)
├── photo-picker.html   ← Tool for Rivka to review + submit photos
├── CNAME               ← aji-fruit-farm.lk
├── README.md           ← Project context for collaborators
├── OWNER-GUIDE.md      ← Plain-English guide for Aji
└── SESSION-LOG.md      ← Claude Code session history
```
