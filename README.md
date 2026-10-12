# Salman Ahmed — Portfolio Website

A modern, responsive one-page portfolio for **Salman Ahmed**, a growth & paid-media
strategist. Built as a fast, dependency-free static site (HTML, CSS, vanilla JS) that
you can host anywhere.

## ⚠️ Before publishing

The page still contains template content. Replace or remove these before the
site goes live or is linked from a profile:

- [ ] Headshot at `assets/salman-ahmed.jpg`
- [ ] Stats in the *Results* section (`data-target` values) — use real, verifiable numbers
- [ ] Case studies in the *Work* section — real projects only
- [ ] Testimonials — real client quotes, used with permission
- [ ] Email, WhatsApp and social links
- [ ] Contact form `action` (it has no backend yet)

## 📸 Add your photo (important)

The site is already wired to use your photo — you just need to drop the file in:

1. Save your headshot as **`assets/salman-ahmed.jpg`** (square works best, ~500×500 or larger).
2. That's it. The hero and About sections pick it up automatically.

Until that file exists, a styled placeholder is shown, so the site always looks complete.
Prefer a different filename or `.png`? Update the two `<img src="...">` tags in `index.html`.

## 🗂 Structure

```
.
├── index.html                     # All page content / sections
├── css/styles.css                 # Design system + responsive layout
├── js/main.js                     # Nav, scroll reveals, counters, form
├── assets/
│   ├── salman-ahmed.jpg           # ← add your photo here
│   ├── placeholder-portrait.svg   # fallback shown until the photo is added
│   └── favicon.svg                # "SA" monogram favicon
└── README.md
```

## ✏️ Make it yours

Everything below is placeholder copy you can edit freely in `index.html`:

- **Stats** in the *Results* section (`data-target` values) — swap in your real numbers.
- **Case studies** in the *Work* section — replace with your actual projects.
- **Testimonials** — use real client quotes (with permission).
- **Contact details** — update the email, WhatsApp link, and social URLs.

### Wire up the contact form

The form validates on the client but has no backend yet. Point it at a form service
(e.g. Formspree, Getform, Basin) or your own endpoint by setting the form's `action`
and `method`, or by sending the values from `js/main.js`.

## 🚀 Run locally

It's a static site — just open `index.html`, or serve the folder:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## 🌐 Deploy

Drag-and-drop the folder to Netlify, or push to GitHub and enable GitHub Pages / Vercel.
No build step required.

This repository has no package manager or build tooling, so it has no CI
workflow or Dependabot version-update config. Add them if a build step or npm
dependencies are introduced later.
