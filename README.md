# MeshCon · Tech Support That Actually Shows Up
### Source code for MeshCon Technical Solutions, a Chicago-based business providing expert on-site tech support, computer repair, and WiFi networking. Professional IT solutions delivered directly to your door. Live at: https://www.meshcon.tech

[!Version](https://github.com/crazykat8091/meshcon)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)
[![Live Site](https://img.shields.io/badge/Live-meshcon.tech-blue?style=flat-square)](https://www.meshcon.tech)

---

## What is MeshCon?
MeshCon is born from the belief that professional tech support should be personal, precise, and—most importantly—convenient. Founded by Bodin Praphanthongchai (Pete), MeshCon brings over 30 years of systems engineering expertise directly to the doorsteps of homes and small businesses across the Chicago area. We specialize in cutting through the jargon to solve the "frustrating" problems: dead WiFi zones, sluggish workstations, and unconfigured smart homes. Our mission is to ensure that your technology serves you, not the other way around, all while keeping your data secure and your devices right where they belong—in your sight.

## 🛠 Tech Stack

| Technology | Usage | Badge |
| :--- | :--- | :--- |
| **HTML5** | Structural Layout & SEO | ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) |
| **CSS3** | Modern Grid/Flexbox & Dark Mode | ![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white) |
| **JavaScript** | UI Interactivity & Theme Logic | ![JavaScript](https://img.shields.io/badge/javascript-%23F7DF1E.svg?style=for-the-badge&logo=javascript&logoColor=black) |
| **SVG** | Scalable Adaptive Branding | ![Vector Graphics](https://img.shields.io/badge/SVG-FFB13B.svg?style=for-the-badge&logo=adobeillustrator&logoColor=white) |

## 📂 Project Structure

```text
.
├── index.html          # Core structural shell and SEO metadata
├── styles.css          # Design system, variables, and responsive layouts
├── app.js              # Theme management, modals, and UI logic
├── blog.html           # Blog index page listing all articles
├── blog/               # Directory for all technical articles
│   ├── wifi-evanston.html
│   ├── arlington-heights.html
│   ├── wifi7-guide.html
│   └── ... (10 articles total)
├── MeshCon-Logo-dark.svg  # Adaptive branding for dark interfaces
├── MeshCon-Logo-light.svg # Adaptive branding for light interfaces
├── site.webmanifest    # PWA and browser configuration
└── README.md           # Project documentation
```

## 🚀 Getting Started

### Run Locally
Since MeshCon is a static site with no heavy dependencies, you can run it using any local development server.

1. **Clone the repository:**
   ```bash
   git clone https://github.com/crazykat8091/meshcon.git
   ```
2. **Navigate to the directory:**
   ```bash
   cd meshcon
   ```
3. **Start a local server:**
   Using Node.js/NPM (Live Server):
```bash
npx serve .
```

### Running Locally
```bash
npm start
```

The server will start at `http://localhost:3000`

### GitHub Pages Deployment

#### Option 1: GitHub Pages Static Site (Recommended for Testing)
1. Push code to GitHub repository
2. Go to repository **Settings → Pages**
3. Select `main` branch as source
4. Site will be available at: `https://www.meshcon.tech/`

**Note:** The `<base>` tag in `index.html` is configured for `/meshcon/`. The Node.js backend (chatbot API) won't work on GitHub Pages static hosting; you'll need a backend service like Vercel for the AI features to function.

## 🌐 DNS Configuration (Squarespace)
To point `www.meshcon.tech` to this repository, you must **first delete all default Squarespace DNS records** (specifically those pointing to `ext-cust.squarespace.com`), then add these:

| Type | Host | Points To |
| :--- | :--- | :--- |
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | crazykat8091.github.io |

### ⚠️ Troubleshooting "InvalidCNAMEError" (Site works, but error shows)
If the site is accessible but GitHub still displays an error:
1. **Force a Re-check:** Remove the domain in GitHub Pages settings, save, and re-add it. This clears GitHub's DNS cache.
2. **Check for "Squarespace Defaults":** In Squarespace, ensure you have clicked "Delete Defaults" if that option is visible. Any record pointing to `ext-cust.squarespace.com` will cause this error.
3. **Verify CNAME Content:** Ensure the `CNAME` file in your repo contains `www.meshcon.tech` (not just `meshcon.tech`).
4. **Check for 'A' Record Conflicts:** Ensure there are no other 'A' records besides the four GitHub IPs.
5. **Wait for SSL:** The "Invalid" error often persists until the SSL certificate is fully issued. Once you can check "Enforce HTTPS", the error usually disappears.

## 📋 Deployment Checklist
### Before Going Live:
- [x] **Update Phone Number:** Phone number confirmed: +1 224-368-9525
- [x] **Update WhatsApp Link:** Integrated `wa.link/5wvtlp`
- [x] **Configure Formspree:** Integrated with ID `xeedzoqy` and verified testing
  - Sign up at [formspree.io](https://formspree.io)
  - Create a new form and get your form ID
  - Replace `xeedzoqy` in `index.html` (Contact Modal form action)
  - Test email submissions in contact modal
- [x] **Add Google Site Verification:** Update `google-site-verification` meta tag
- [x] **Privacy Contact:** Integrated `whatsapp-qr.png` for secure scanning
- [x] **Setup Google Analytics:** GA4 integrated (Measurement ID: G-XXXXXXXXXX)
- [x] **Social Media Links:** Verified: Active links only; placeholders removed
- [x] **Ensure og-image.jpg is present:** og-image.jpg confirmed at 1200x630px
- [x] **Custom Domain:** 
  - Add a `CNAME` file containing `www.meshcon.tech` to root (if using GitHub Pages)
  - Update absolute URLs in meta tags from `https://www.meshcon.tech/` to your domain
- [ ] **API Key Security:** 
  - Use environment variables in production
  - Never commit API keys to repository
  - Rotate keys if accidentally exposed

### 🔜 Upcoming
- [ ] Suburb landing pages (Arlington Heights, Evanston, Schaumburg)
- [ ] Blog section (3-5 local SEO posts)
- [ ] Google Business Profile (pending verification)
- [ ] AI Chatbot re-enable (pending Vercel backend deployment)

### Testing & Validation:
- [ ] **Performance:** Run [PageSpeed Insights](https://pagespeed.web.dev/) - Target: 90+/100
- [ ] **Social Preview:** Use [Facebook Sharing Debugger](https://developers.facebook.com/tools/debug/) to verify OG image
- [ ] **Mobile Responsive:** Test on iPhone/Android in Chrome DevTools
- [ ] **Chatbot:** (Disabled) Update UI when AI backend is ready
- [ ] **Accessibility:** Check WCAG 2.1 AA compliance with [axe DevTools](https://www.deque.com/axe/devtools/)
- [ ] **DNS:** Verify domain resolves correctly and SSL cert is valid

### 🛠 Production Tools
- **Social Debugger:** [Facebook Sharing Debugger](https://developers.facebook.com/tools/debug/) (Use "Scrape Again" if preview doesn't update)
- **Performance Check:** [PageSpeed Insights](https://pagespeed.web.dev/)
- **SEO Check:** [Google Search Console](https://search.google.com/search-console/)
- **Accessibility:** [axe DevTools](https://www.deque.com/axe/devtools/)
- **SSL/HTTPS:** [SSL Labs](https://www.ssllabs.com/ssltest/)

## 🤝 Contact
**Bodin Praphanthongchai (Pete)**  
Email: info@meshcon.tech  
Phone: +1 224-368-9525  
Website: www.meshcon.tech (Your trusted local tech expert)

---
*Developed by Bodin Praphanthongchai (Pete) · Version 1.55*