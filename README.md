# MeshCon · Tech Support That Actually Comes To You

[![Live Site](https://img.shields.io/badge/Live%20Site-meshcon.tech-ff8a2a?style=flat-square&logo=google-chrome&logoColor=white)](https://www.meshcon.tech)
[![Version](https://img.shields.io/badge/Version-1.54-0e0e0e?style=flat-square)](...)
[![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)](LICENSE)
[![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-181717?style=flat-square&logo=github)](https://pages.github.com)
[![Stack](https://img.shields.io/badge/Stack-HTML5%20%7C%20CSS3%20%7C%20JS-f7df1e?style=flat-square)](https://github.com/crazykat8091/meshcon)

> **On-site tech support for Chicago's North Side and suburbs — no jargon, no hidden fees, just real help at your door.**

---

## 🧭 What Is MeshCon?

MeshCon is a solo, expert-led tech support service founded by **Bodin Praphanthongchai (Pete)**. With 30+ years of hands-on experience, Pete brings professional IT support directly to homes and small businesses within a 35-mile radius of Chicago — no shop drop-offs, no confusing tech-talk, no surprises on the bill.

This repository contains the complete source code for the [meshcon.tech](https://www.meshcon.tech) website: a high-performance, zero-dependency static site built with pure HTML5, CSS3, and Vanilla JavaScript.

---

## 🛠 Tech Stack

| Layer | Technology |
|---|---|
| Structure | HTML5 (Semantic, Accessible) |
| Styling | CSS3 — Flexbox & Grid, Custom Properties |
| Interactivity | Vanilla JavaScript ES6+ |
| Graphics | SVG (adaptive dark/light mode) |
| Forms | Formspree (ID: `xeedzoqy`) |
| Hosting | GitHub Pages + Custom Domain |
| DNS | Squarespace → GitHub Pages (A + CNAME records) |

---

## ✨ Key Features

- **Zero-dependency architecture** — no frameworks, no build tools, sub-second load times
- **Adaptive SVG branding** — logos and business cards auto-switch for dark/light mode and print
- **Fully responsive** — optimized from 375px mobile to 1440px+ desktop
- **Contact system** — Formspree email form + WhatsApp direct link + click-to-call phone
- **Local SEO ready** — semantic HTML, meta tags, OG/Twitter cards, sitemap, robots.txt, Google site verification
- **PWA-ready manifest** — `site.webmanifest` configured for mobile add-to-homescreen

---

## 🎨 Brand Identity

| Token | Value | Use |
|---|---|---|
| Primary Accent | `#ff8a2a` | Dark mode CTA, highlights |
| Accessible Accent | `#bf5a00` | Light mode CTA, text links |
| Dark Surface | `#0e0e0e` | Dark mode background |
| Light Surface | `#fcfaf8` | Light mode background |
| Brand Font | Plus Jakarta Sans | Headings |
| UI Font | Inter | Body text |
| Technical Font | JetBrains Mono | Code/status labels |
| Signature Font | Caveat | Accent handwriting |

---

## 📂 Project Structure

```
meshcon/
├── index.html              # Entry point (redirects to MeshCon.html)
├── MeshCon.html            # Core page — structure, SEO metadata, all sections
├── styles.css              # Complete design system & responsive layouts
├── app.js                  # Interactivity: theme toggle, form handling, chat widget
├── MeshCon-Logo-dark.svg   # Logo for dark mode
├── MeshCon-Logo-light.svg  # Logo for light mode
├── MeshCon-Logo-dark.png   # PNG fallback (dark)
├── MeshCon-Logo-light.png  # PNG fallback (light)
├── business_card_dark.svg  # Printable business card (dark)
├── business_card_light.svg # Printable business card (light)
├── circuit-board-detail.jpg# Gallery/precision section hero image
├── og-image.jpg            # Social share preview (1200×630px)
├── whatsapp-qr.png         # WhatsApp QR code for contact section
├── site.webmanifest        # PWA manifest
├── sitemap.xml             # XML sitemap for search engines
├── robots.txt              # Crawler directives
├── ads.txt                 # Ad network authorization
├── CNAME                   # Custom domain: www.meshcon.tech
└── README.md               # This file
```

---

## 🚀 Getting Started

### Run Locally

```bash
# Clone the repo
git clone https://github.com/crazykat8091/meshcon.git
cd meshcon

# Install dependencies (local dev server only)
npm install

# Start local server at http://localhost:3000
npm start
```

> **Note:** The site is a static HTML file. You can also just open `MeshCon.html` directly in a browser for a quick preview without Node.

### Deploy to GitHub Pages

1. Push to the `main` branch
2. Go to **Settings → Pages**
3. Set source to `main` branch, root `/`
4. Add custom domain `www.meshcon.tech`
5. Check **Enforce HTTPS** once SSL certificate is issued

---

## 🌐 DNS Configuration

DNS is managed through **Squarespace**. Delete all default Squarespace records first, then add:

| Type | Host | Points To |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | crazykat8091.github.io |

---

## 📋 Deployment Checklist

### ✅ Completed
- [x] Phone number live: `+1 224-368-9525`
- [x] WhatsApp link active: `wa.link/6hs9t7`
- [x] Formspree contact form integrated (ID: `xeedzoqy`)
- [x] Google Site Verification meta tag added
- [x] Custom domain configured: `www.meshcon.tech`
- [x] OG image confirmed: `og-image.jpg` at 1200×630px
- [x] Canonical URL, OG tags, Twitter card all set
- [x] `sitemap.xml` and `robots.txt` present
- [x] Google Search Console connected

### 🔜 In Progress / Upcoming
- [ ] Google Business Profile (pending postcard verification)
- [ ] Google Analytics GA4 setup
- [ ] Social media accounts (Facebook, Instagram priority)
- [ ] LocalBusiness JSON-LD schema in `<head>`
- [ ] Suburb landing pages (Arlington Heights, Evanston, Schaumburg)
- [ ] Blog section (local SEO content)
- [ ] AI Chatbot re-enable (pending Vercel backend)
- [ ] PageSpeed Insights score — target 90+

---

## 🔧 Troubleshooting

### "InvalidCNAMEError" on GitHub Pages
1. In Squarespace DNS, click **Delete Defaults** to remove any `ext-cust.squarespace.com` records
2. In GitHub Pages Settings, remove and re-add the custom domain to force a DNS re-check
3. Confirm `CNAME` file contains exactly `www.meshcon.tech`
4. Wait for SSL cert issuance — the error often clears once HTTPS is enforced

---

## 🤝 Contact

**Bodin Praphanthongchai (Pete)**
- 🌐 [www.meshcon.tech](https://www.meshcon.tech)
- 📧 [info@meshcon.tech](mailto:info@meshcon.tech)
- 📞 [+1 224-368-9525](tel:+12243689525)
- 💬 [WhatsApp](https://wa.link/6hs9t7)

---

*MeshCon Technical Solutions · Chicago, IL · Version 1.29*
*© 2026 Bodin Praphanthongchai · MIT License*
