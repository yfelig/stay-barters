# Your Website — Owner Guide

Welcome! This guide explains how to update your website. You don't need to know how to code.

---

## How to update text

1. Open `index.html` in any text editor (TextEdit on Mac, Notepad on Windows)
2. Use **Find & Replace** (Cmd+H / Ctrl+H) to change text
3. Save the file
4. Push the change to GitHub (or ask Yair) — the site updates automatically within a minute

---

## How to update photos

1. Optimize your new photo to under 500KB (use [squoosh.app](https://squoosh.app) — free)
2. Save it to the `photos/` folder with the same filename as the one you're replacing
3. Push to GitHub — the site updates automatically

---

## How to change the booking message

In `index.html`, find the two lines that start with:
```
href="https://wa.me/...
```

Edit the text after `?text=` — this is what guests see pre-filled in WhatsApp when they tap the button. Spaces must be written as `%20`.

Example: `Hello!%20I'm%20interested%20in%20booking%20a%20stay.`

---

## Your files

```
index.html     ← all the text content
style.css      ← colors and layout (don't touch unless you know CSS)
script.js      ← gallery behavior (don't touch)
photos/        ← all images
```

---

## Need help?

Reach Yair at: yair.felig@uglabs.io

---

*Built with care by Stay Barters — Yair & Rivka Felig.*
