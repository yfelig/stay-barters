# Stay Barters

**We stay. We shoot. We build. You keep it.**

Stay Barters is a personal venture by Yair & Rivka Felig. We travel, find interesting places to stay, and offer the owners a trade: Rivka photographs the property and Yair builds a professional landing page — in exchange for a free or discounted stay.

The owner walks away with a real online presence that drives direct bookings via WhatsApp — no Airbnb or Booking.com commission.

---

## What each place gets

- A single-page landing site with their story, photos, facilities, and a direct WhatsApp booking link
- Their own GitHub repository (they own the code forever)
- A custom domain for the first year (we cover the cost, ~$10–15)
- A handoff guide so they can update text and photos themselves

---

## How it works

### 1. During the stay
- Rivka shoots the property — exterior, interior, details, atmosphere
- Yair interviews the owner: their story, what makes the place special, what's included
- We collect: owner's WhatsApp number, preferred booking message, any rules/notes

### 2. Building the page
- Copy `template/` into a new folder named after the property (e.g. `mango-farm-galilee/`)
- Fill in all `[PLACEHOLDERS]` in `index.html`
- Drop Rivka's optimized photos into `photos/`
- Test locally, share preview link for owner feedback

### 3. Handoff
- Create a new **public** GitHub repo under the owner's account (or ours, transferred to them)
- Push the site
- Buy the domain (Namecheap/Cloudflare), point DNS to GitHub Pages
- Enable GitHub Pages in repo settings → `main` branch → `/ (root)`
- Hand over the repo link + login credentials + `OWNER-GUIDE.md`

### 4. Log the stay
- Add an entry to `stays/log.md` with property name, dates, location, and live URL

---

## Template

The `template/` folder is the base for every new property. It contains:

```
template/
├── index.html        ← single-page site, fill in all [PLACEHOLDERS]
├── style.css         ← styles, customize accent color per property
├── script.js         ← minimal JS: smooth scroll + gallery lightbox
├── photos/           ← drop optimized images here (WebP preferred)
└── OWNER-GUIDE.md    ← plain-English guide for the owner
```

### Placeholders to fill in `index.html`

| Placeholder | What to put |
|-------------|-------------|
| `[PLACE_NAME]` | Name of the property |
| `[TAGLINE]` | One evocative sentence |
| `[OWNER_NAME]` | Owner's first name |
| `[OWNER_STORY]` | 2–3 sentences about them and the place |
| `[PLACE_STORY]` | What makes this place unique |
| `[FACILITIES_LIST]` | Array of facility items in the HTML |
| `[WHATSAPP_NUMBER]` | International format, no `+`, no spaces (e.g. `972521234567`) |
| `[BOOKING_MESSAGE]` | Pre-filled WhatsApp message (URL-encoded) |
| `[LOCATION]` | Region/area for the footer |
| `[ACCENT_COLOR]` | Hex color in `style.css` that matches the property's vibe |

---

## Stack

- Pure HTML + CSS + vanilla JS — no build step, no dependencies
- Hosted on GitHub Pages (free)
- Custom domain via Namecheap or Cloudflare (~$10–15/yr, first year on us)

---

## Stays log

See [`stays/log.md`](stays/log.md) for all completed stays.

---

*Yair & Rivka Felig — building the web one stay at a time.*
