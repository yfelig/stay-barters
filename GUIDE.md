# Stay Barters — The Playbook

A step-by-step guide for building a professional website for a place, in exchange for a free or discounted stay.

**The concept in one sentence:** You arrive as a guest, leave as a collaborator — the owner gets a website that drives direct bookings, you get the stay paid in skill.

---

## Overview

| Phase | What happens | When |
|-------|-------------|------|
| 1. Find | Spot a property that would benefit | Before booking |
| 2. Pitch | Propose the trade | Via email or in-person |
| 3. Prepare | Research, plan the content | Before arrival |
| 4. Interview | Capture the story | Day 1 of the stay |
| 5. Shoot | Photograph everything | Days 1–2 |
| 6. Build | Code the site | During or after the stay |
| 7. Launch | Domain, GitHub Pages, handoff | Final day or within a week |

Typical stay needed: **2–3 nights minimum.** Longer for complex properties.

---

## Phase 1 — Finding the Right Property

Look for places that have something real but no web presence (or a bad one):

**Good signs:**
- Listed on Airbnb/Booking but no standalone website
- Unique story or setting (farm, lake, jungle, family-run)
- Owner is hands-on and communicates personally
- Reviews exist but guests have to dig to find them
- Priced reasonably (not a 5-star resort — they already have agencies)

**Red flags:**
- Already has a good website → no trade value
- Corporate-owned → no owner relationship
- No personality / nothing to tell a story about

---

## Phase 2 — The Pitch

Keep it simple and human. This works best in person or over WhatsApp.

**What to say:**
> "I build websites for places I love staying at. I'd like to trade — I'll build you a professional website that helps you get direct bookings (no Airbnb commission), in exchange for [X nights]. You keep everything — the code, the domain, all of it."

**What you're offering:**
- A 4-page website with their story, photos, facilities, reviews, and a direct WhatsApp booking link
- A GitHub repo they own forever
- A custom domain (first year covered, ~$10–20)
- A handoff guide so they can update it themselves

**Typical trade:** 2–4 nights depending on property size. Agree upfront.

---

## Phase 3 — Preparation (Before Arrival)

- [ ] Check if they have existing Airbnb/Booking/TripAdvisor — note their reviews, star rating, review count
- [ ] Note any social media (Instagram, Facebook)
- [ ] Think about the domain name (e.g. `aji-fruit-farm.lk`, `mamadjuice.co.il`)
- [ ] Bring: a camera or phone with a good lens, a tripod if possible, a notebook
- [ ] Clone or copy the `template/` folder, name it after the property

---

## Phase 4 — The Interview

Do this on Day 1. Record audio if they're comfortable with it, or take notes. Ask in their language if possible — translate later.

### Origin story
- How long have you been running this place?
- How did you come to own it / start this?
- What was here before?
- What changed along the way?

### What makes it special
- What do you want guests to feel when they arrive here?
- What do guests say when they leave?
- What can they get here that they can't get anywhere else nearby?

### The practical stuff
- What's included in the price? (Breakfast? Transfers? Activities?)
- What's check-in / check-out?
- What activities do you offer on-site?
- What's nearby that you can arrange? (safari, horse riding, day trips)
- Do you have a pet / family members / staff involved?

### Honest expectations
- What should guests know before they arrive? (cold showers? no restaurant nearby? nature very close?)
- Who is this place NOT for?

### Booking logistics
- What's your WhatsApp number?
- What message do you want guests to send when they inquire?
- Do you have a minimum stay?
- Do you have seasonal pricing?

### Reviews
- Are you on Airbnb / Booking / TripAdvisor?
- Can I use real quotes from your reviews on the website?
- What's your star rating and approximate review count?

### Social / contacts
- Do you have Instagram or Facebook?
- Do you want a contact email on the site?

---

## Phase 5 — Photography

Shoot across the stay, not all at once. Golden hour (6–8am, 4–6pm) is mandatory for outdoor shots.

### Must-have shots

**Hero / establishing (2–3 shots)**
- The full property from a distance — landscape, farm, building in its setting
- Golden hour light ideally
- This becomes the homepage hero — needs to be stunning

**The setting (4–6 shots)**
- The natural environment: lake, garden, orchard, jungle, view
- Atmosphere: mist on water, fruit on trees, animals
- Guests want to feel the place before they arrive

**Exterior — the cottage/room (3–4 shots)**
- Building from outside, set in its surroundings
- The entrance / door
- Veranda or outdoor seating
- The path to the room

**Interior — the room (4–6 shots)**
- Full room from doorway (zoomed out, shows everything)
- The bed — clean linen, good light
- Any unique feature (handmade furniture, concrete walls, unusual architecture)
- Seating area if separate

**The bathroom (2–3 shots)**
- Full bathroom shot
- If unusual (open-air, outdoor shower, vessel sink) — this is a selling point, get a hero shot of it

**Food (4–6 shots)**
- The breakfast spread — everything on the table at once
- Close-up of something local or distinctive (hoppers, fresh fruit, eggs)
- Any Sri Lankan / local dish if they cook on request
- Fresh produce if farm-grown

**The host (2–3 shots)**
- Natural portrait — not posed, caught while doing something (tending the farm, pouring tea, carrying kayaks)
- With family if comfortable
- A candid that shows their personality

**Activities (1–2 shots per activity)**
- Kayaking, swimming, bikes, whatever's on offer
- Nearby safari / attraction (if you go)
- Horse riding, hiking, etc.

**Details (5–10 shots)**
- Fruit on the tree, mangos in a basket
- Architecture textures (concrete, teak, rattan)
- Morning light through trees
- These fill photo grids and carousels — collect as many as possible

### Technical notes
- Shoot in landscape (horizontal) for hero images and split sections
- Shoot in portrait (vertical) for bathroom and some room shots
- No people unless the host specifically agrees to be photographed
- Don't over-edit — keep colors natural, just lift shadows slightly

---

## Phase 6 — Building the Site

### Stack

| Layer | Choice | Why |
|-------|--------|-----|
| HTML/CSS/JS | Vanilla, no framework | No build step, owner can edit directly |
| Fonts | Cormorant Garamond + Inter (Google Fonts) | Boutique/editorial feel |
| Hosting | GitHub Pages | Free, reliable, HTTPS auto-provisioned |
| Domain | Namecheap / Cloudflare / local registrar | ~$10–20/yr |
| Booking CTA | WhatsApp link via `wa.me/` | No integration needed |
| Map | Google Maps embed | Free, no API key for basic embed |
| Photos | JPG optimized to ~200–400KB | Fast loading, no CDN needed |
| Reviews | Static HTML (copy-paste from Airbnb/TripAdvisor) | No third-party widget |

### Page structure (the 4-page model)

```
index.html       ← Homepage — the full story in sections
rooms.html       ← The accommodation — photo slider + specs
place.html       ← The setting — farm, lake, nature, food
story.html       ← The owner — origin, journey, why they built this
```

A minimal build can compress to **1 page** (everything on index.html). Use 4 pages for richer properties.

---

### index.html — Section by Section

| Section | What it does | Key element |
|---------|-------------|-------------|
| **Nav** | Logo + links + Book Direct button | WhatsApp link on the button |
| **Hero** | Full-viewport photo + property name | `object-fit: cover`, animated scroll arrow |
| **Welcome** | 2-column: copy left, photo right | Sets the scene in 3 sentences |
| **Meet the host** | 2-column: photo left, copy right | Host quote in italic |
| **Rooms teaser** | 3-photo grid linking to rooms.html | Main + 2 side images |
| **The setting** | 2-column: photo + copy | Lake/garden/nature |
| **Activities** | 3-column cards with photos | Distance badge overlay |
| **Food** | 2-column: copy + photo | Breakfast / local food |
| **Reviews** | Rotating quotes + 5-star rating | Dot navigation carousel |
| **Find Us** | Dark bg: address + WhatsApp button + map | Google Maps embed |
| **Footer** | Name, social icons, attribution | |
| **Floating WhatsApp** | Fixed bottom-right button | Always visible |

---

### rooms.html — The Accommodation Page

- Large photo slider (full viewport width, 70–80vh height)
- 2-column specs: description left, "What's Included" list right
- Emoji icons for amenity list (bed, wifi, AC, breakfast, etc.)
- "Honest note" strip: what this place actually is (trust-builder)
- Dark CTA section at bottom: Book Directly via WhatsApp

---

### place.html — The Setting

- Hero image (60–70vh)
- Photo grids (2-col and 3-col) between content sections
- Split sections for lake/nature, activities, food
- Horizontal food scroll carousel
- Book CTA at bottom

---

### story.html — The Owner Story

- Full-height portrait hero
- 3-act narrative: Before → The crisis/change → Now
- Portrait split (photo + text)
- Full-width family/atmosphere photo strip
- Pull quote (large centered italic)
- "See the rooms →" bridge before the book CTA

---

### Essential elements on every page

```html
<!-- Floating WhatsApp button — always visible -->
<a class="wa-float" href="https://wa.me/[NUMBER]?text=[ENCODED_MESSAGE]" target="_blank">
  [WhatsApp SVG icon]
</a>

<!-- Nav booking button -->
<a class="nav-wa" href="https://wa.me/[NUMBER]?text=[ENCODED_MESSAGE]" target="_blank">
  Book Direct
</a>

<!-- Footer CTA section (dark bg) -->
<section class="room-book">
  <h2>Book Directly with [Owner]</h2>
  <p>No platform, no fees. Message [Owner] on WhatsApp — they reply fast.</p>
  <a class="btn-wa" href="https://wa.me/[NUMBER]?text=[ENCODED_MESSAGE]">
    +[NUMBER]
  </a>
</section>
```

**WhatsApp link format:**
```
https://wa.me/[COUNTRY_CODE][NUMBER]?text=Hi%20[Name]%2C%20I%20found%20your%20farm%20online%20and%20I%27d%20love%20to%20book%20a%20stay.
```

**Reviews carousel JavaScript:**
- Store quotes as a JS array: `{ text: "...", author: "Name, Country" }`
- Rotate on dot click with opacity fade transition
- Show 5–6 real quotes pulled from Airbnb/TripAdvisor
- Display: ★★★★★ in gold (`#c8952e`) + platform count below

---

### Design system (Aji model — proven to work)

```css
:root {
  --bg:       #f0ede4;   /* warm linen */
  --bg-alt:   #e8e2d6;   /* slightly darker for alternating sections */
  --bg-dark:  #1b3826;   /* deep forest green — CTAs, footer */
  --text:     #18180f;   /* near-black */
  --muted:    #6b6856;   /* body copy, labels */
  --border:   #d4cec3;   /* dividers */
  --wa-green: #25d366;   /* WhatsApp button */
  
  --font-display: 'Cormorant Garamond', Georgia, serif;  /* headings */
  --font-body:    'Inter', system-ui, sans-serif;        /* body */
}
```

Adapt `--bg-dark` to match the property's character:
- Farm/jungle → deep green (`#1b3826`)
- Desert/Negev → warm terracotta (`#7a3b2e`)
- Coastal → navy (`#1a2e4a`)
- Vineyard → burgundy (`#4a1e2e`)

---

## Phase 7 — Domain & Deployment

### GitHub Pages setup
1. Create a public repo: `[property-slug]` (e.g. `ajis-mango-farm`)
2. Push all files to `main` branch
3. Go to repo Settings → Pages → Source: `main` / `/ (root)` → Save
4. GitHub gives you: `[username].github.io/[repo-name]`

### Custom domain
1. Buy the domain:
   - International: [Namecheap](https://namecheap.com) or [Cloudflare](https://cloudflare.com) — ~$10–15/yr for `.com`
   - Country-specific: local registrar (e.g. Register.lk for `.lk`, ~$20–30/yr)
2. In the registrar's DNS settings, add:
   ```
   A    @    185.199.108.153
   A    @    185.199.109.153
   A    @    185.199.110.153
   A    @    185.199.111.153
   CNAME www  [username].github.io
   ```
3. In GitHub Pages settings → Custom domain → enter the domain → Save
4. GitHub auto-provisions HTTPS (takes ~1 hour after DNS propagates)
5. Verify with: `dig [domain] +short` — should return the 4 IPs above

### Add a CNAME file
Create a file called `CNAME` in the repo root with one line:
```
your-domain.com
```
This survives re-deployments.

---

## Phase 8 — Handoff

**What the owner gets:**
- [ ] GitHub repo URL (public, they can clone or fork)
- [ ] `OWNER-GUIDE.md` — plain-English instructions for updating text and photos
- [ ] Domain credentials (if you bought it for them — transfer the domain to their registrar account)
- [ ] Their WhatsApp number confirmed working in all booking CTAs
- [ ] HTTPS confirmed active
- [ ] Added as GitHub collaborator with push access

**README to write in the repo:**
Include: what the site is, the 4-page structure, photo inventory (which photo is in which slot), how to update, Claude instructions for future AI-assisted updates.

---

## Time & Cost Estimates

| Item | Time | Cost |
|------|------|------|
| Interview | 1–2 hours | — |
| Photography | 2–4 hours | — |
| Photo editing / resize | 1–2 hours | — |
| Building (simple 1-page) | 4–8 hours | — |
| Building (4-page model) | 12–20 hours | — |
| Domain (first year) | — | $10–30 |
| Hosting (GitHub Pages) | — | Free |
| **Total you cover** | **~16–28 hours** | **~$10–30** |

A 3-night stay at a $50/night guesthouse = $150 of value for ~$20 in costs.

---

## Tips from the First Build (Aji Fruit Farm)

- **Get the real story.** The most compelling copy comes directly from the owner's words — especially the crisis/turning-point chapter. Don't write generic "welcome to our beautiful property" copy.
- **Cold showers = a feature, not a bug.** Honest expectations build trust. Put the disclaimer ("showers are cold water, nature is close — not a 5-star resort") directly on the rooms page. It pre-qualifies visitors and reduces disappointment.
- **WhatsApp pre-fills convert.** The booking message should be pre-written and URL-encoded. Visitors send it with one tap.
- **4 pages > 1 page.** The 4-page model lets each page tell a complete story and rank separately in search. The story page especially drives emotional connection.
- **Don't use close-up abstract shots as teaser images.** Every photo in a grid or teaser must answer one of: *What does the setting look like? What is the room like? What makes it unique?* A blurry door handle answers none of these.
- **Review quotes need to be real.** Copy exact quotes from Airbnb/TripAdvisor reviews. Attribution ("— Momoyo, Japan") makes them credible. Ask permission or note the platform source.
- **Rivka shoots, Yair builds.** Keep the roles clean. Photographer doesn't code, builder doesn't art-direct the shots.

---

## Reference

**GitHub Pages IPs:**
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

**WhatsApp link builder:**
`https://wa.me/[NUMBER]?text=[URL-ENCODED-MESSAGE]`
Use any URL encoder to encode the message text.

**Google Maps embed:**
```html
<iframe
  src="https://maps.google.com/maps?q=[LOCATION]&t=&z=13&ie=UTF8&iwloc=&output=embed"
  width="100%" height="100%" style="border:0;" allowfullscreen loading="lazy">
</iframe>
```

**Font import:**
```html
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300;1,400&family=Inter:wght@300;400;500&display=swap" rel="stylesheet" />
```

**Photo optimization:**
- Target: 200–400KB per image
- Format: JPG for photos, SVG for icons
- Max dimensions: 2400px wide for hero, 1600px for others
- Tools: [Squoosh.app](https://squoosh.app) (free, browser-based)
