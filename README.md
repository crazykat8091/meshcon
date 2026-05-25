# MeshCon · Tech Support That Actually Comes To You

[![Live Site](https://img.shields.io/badge/Live%20Site-meshcon.tech-ff8a2a?style=flat-square&logo=google-chrome&logoColor=white)](https://www.meshcon.tech)
[![Version](https://img.shields.io/badge/Version-1.55-0e0e0e?style=flat-square)](https://github.com/crazykat8091/meshcon/commits/main)
[![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)](LICENSE)
[![Hosted on GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-181717?style=flat-square&logo=github)](https://pages.github.com)
[![Stack](https://img.shields.io/badge/Stack-HTML5%20%7C%20CSS3%20%7C%20Vanilla%20JS-f7df1e?style=flat-square)](#-tech-stack)

> **Expert on-site tech support for Chicago's North Side and suburbs — no jargon, no hidden fees, just real help at your door.**

---

## 🧭 What Is MeshCon?

MeshCon is a solo, expert-led tech support business founded by **Bodin Praphanthongchai (Pete)**. With 30+ years of hands-on experience, Pete brings professional IT support directly to homes and small businesses within a 35-mile radius of Chicago — no shop drop-offs, no confusing tech-talk, no bill surprises.

This repository contains the complete source code for [meshcon.tech](https://www.meshcon.tech): a high-performance, zero-dependency static website built with pure HTML5, CSS3, and Vanilla JavaScript, hosted on GitHub Pages with a custom domain.

---

## 🛠 Tech Stack

| Layer | Technology |
|---|---|
| Structure | HTML5 (Semantic, Accessible) |
| Styling | CSS3 — Flexbox & Grid, Custom Properties |
| Interactivity | Vanilla JavaScript ES6+ |
| Graphics | SVG (adaptive dark/light mode + print) |
| Forms | Formspree (ID: `xeedzoqy`) |
| Hosting | GitHub Pages + Custom Domain |
| DNS | Squarespace → GitHub Pages (A + CNAME records) |

---

## ✨ Key Features

- **Zero-dependency architecture** — no frameworks, no build pipeline, sub-second load times
- **Adaptive SVG branding** — logos and business cards auto-switch for dark/light mode and print
- **Fully responsive** — optimized from 375px mobile to 1440px+ desktop
- **Blog section** — local SEO content at `/meshcon/blog.html`
- **Multi-channel contact** — Formspree email form + WhatsApp direct link + click-to-call phone
- **Local SEO ready** — semantic HTML, meta tags, OG/Twitter cards, sitemap, robots.txt, Google Search Console verified
- **PWA-ready** — `site.webmanifest` configured for mobile add-to-homescreen

---

## 🎨 Brand Identity

| Token | Value | Use |
|---|---|---|
| Primary Accent | `#ff8a2a` | Dark mode CTAs, highlights |
| Accessible Accent | `#bf5a00` | Light mode CTAs, links |
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
├── index.html                  # Main entry point — full site
├── MeshCon.html                # Legacy shell (redirects to index.html)
├── styles.css                  # Complete design system & responsive layouts
├── app.js                      # Theme toggle, form handling, chat widget
├── meshcon/
│   ├── blog.html               # Blog — local SEO content
│   ├── MeshCon-Logo-dark.svg   # Logo for dark mode
│   ├── MeshCon-Logo-light.svg  # Logo for light mode
│   ├── MeshCon-Logo-dark.png   # PNG fallback (dark)
│   ├── MeshCon-Logo-light.png  # PNG fallback (light)
│   ├── business_card_dark.svg  # Printable business card (dark)
│   ├── business_card_light.svg # Printable business card (light)
│   ├── circuit-board-detail.jpg# Gallery precision section image
│   └── whatsapp-qr.png         # WhatsApp QR code for contact section
├── og-image.jpg                # Social share preview (1200×630px)
├── site.webmanifest            # PWA manifest
├── sitemap.xml                 # XML sitemap for search engines
├── robots.txt                  # Crawler directives
├── ads.txt                     # Ad network authorization
├── CNAME                       # Custom domain: www.meshcon.tech
├── CHANGELOG.md                # Version history
└── README.md                   # This file
```

---

## 🚀 Getting Started

### Run Locally

```bash
# Clone the repo
git clone https://github.com/crazykat8091/meshcon.git
cd meshcon

# Install dev dependencies (local server only)
npm install

# Start local server at http://localhost:3000
npm start
```

> You can also open `index.html` directly in any browser for an instant preview — no build step needed.

### Deploy to GitHub Pages

1. Push changes to the `main` branch
2. Go to **Settings → Pages**
3. Set source to `main` branch, root `/`
4. Add custom domain `www.meshcon.tech`
5. Enable **Enforce HTTPS** once the SSL certificate is issued

---

## 🌐 DNS Configuration (Squarespace)

Delete all default Squarespace records first, then add:

| Type | Host | Points To |
|---|---|---|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | crazykat8091.github.io |

### Troubleshooting InvalidCNAMEError

1. In Squarespace, click **Delete Defaults** to remove `ext-cust.squarespace.com` records
2. In GitHub Pages Settings, remove and re-add the domain to force a DNS cache clear
3. Confirm `CNAME` file contains exactly `www.meshcon.tech`
4. Wait for SSL certificate issuance — error clears once HTTPS is enforced

---

## 📋 Deployment Status

### ✅ Complete
- [x] `index.html` live as main entry point
- [x] Phone number confirmed: `+1 224-368-9525`
- [x] WhatsApp link active: `wa.link/5wvtlp`
- [x] Formspree contact form integrated (ID: `xeedzoqy`)
- [x] Google Site Verification active
- [x] Custom domain live: `www.meshcon.tech`
- [x] OG image confirmed: `og-image.jpg` at 1200×630px
- [x] Canonical URL, full OG + Twitter card meta tags set
- [x] `sitemap.xml` and `robots.txt` present
- [x] Google Search Console connected
- [x] Blog section live at `/meshcon/blog.html`
- [x] Dark/light mode theme toggle functional

### 🔜 Upcoming
- [ ] LocalBusiness JSON-LD schema in `<head>`
- [ ] Google Analytics GA4 setup
- [ ] Copyright year in footer (`© 2026 MeshCon`)
- [ ] Verify/create social media accounts (Facebook, Instagram priority)
- [ ] Suburb landing pages (Arlington Heights, Evanston, Schaumburg)
- [ ] Google Business Profile (pending postcard verification)
- [ ] AI Chatbot re-enable (pending Vercel backend)
- [ ] PageSpeed Insights — target 90+

---

## 🔧 Production Tools

| Tool | Purpose |
|---|---|
| [PageSpeed Insights](https://pagespeed.web.dev/) | Performance audit — target 90+ |
| [Google Search Console](https://search.google.com/search-console/) | SEO monitoring |
| [Facebook Sharing Debugger](https://developers.facebook.com/tools/debug/) | OG image preview check |
| [axe DevTools](https://www.deque.com/axe/devtools/) | WCAG 2.1 AA accessibility |
| [SSL Labs](https://www.ssllabs.com/ssltest/) | HTTPS certificate validation |

---

## 🤝 Contact

**Bodin Praphanthongchai (Pete)**
- 🌐 [www.meshcon.tech](https://www.meshcon.tech)
- 📧 [info@meshcon.tech](mailto:info@meshcon.tech)
- 📞 [+1 224-368-9525](tel:+12243689525)
- 💬 [WhatsApp](https://wa.link/5wvtlp)

---

*MeshCon Technical Solutions · Chicago, IL · Version 1.55*
*© 2026 Bodin Praphanthongchai · MIT License*
