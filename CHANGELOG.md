# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.55.0] - 2024-12-07

### Added
- **Audit & Optimization**: Comprehensive consistency pass across all 12 HTML files.
- **Code Quality**: Refactored contact modal inline styles into `styles.css`.

### Changed
- **Synchronicity**: Unified all page versions to v1.55.
- **UI Consistency**: Verified social media icon order (FB, IG, X, Discord, WA) globally.

## [1.54.0] - 2024-12-06

### Added
- **Interactive UI**: Implemented high-performance "Shimmer" and "Pulse" animations for CTA buttons to enhance user engagement.
- **Visual Enhancements**: Added premium gradients and glassmorphism effects to WhatsApp and Email action buttons.

### Changed
- **Mobile Ergonomics**: Increased tap target sizes and optimized button layout for mobile devices.
- **Version Bump**: Global update to version 1.54.0.

## [1.52.0] - 2024-12-05

### Added
- **Performance Audit**: Implemented `fetchpriority="high"` for critical brand assets and enforced `decoding="async"` across all images.
- **Consistency Pass**: Standardized footer signatures and spacing across the root and `/blog/` subdirectory.

### Changed
- **Version Bump**: Global update to version 1.52.0 for production release.

## [1.30.0] - 2024-11-20

### Added
- **Global Audit**: Standardized styling, layout, and scaling across the main site and the `/blog/` subdirectory.
- **Universal Chat**: Integrated the floating WhatsApp/Email chat component into all 10 blog posts for seamless support.
- **Pete's Tone**: Refined all content to use natural human language, removing generic hyphen-based separators.
- **Navigation Fixes**: Restored the SVG back-arrow to blog posts and synchronized header behaviors.

## [1.29.0] - 2024-05-22

### Added
- Implementation of Google Analytics (GA4) for visitor tracking.
- Suburb-specific landing pages for localized SEO.
- New blog post: "Tech Troubles in Arlington Heights? Why Your WiFi is Slow and Your Laptop is Lagging".

### Changed
- Re-enabling and testing the AI Chatbot backend functionality.
- Blog section refactored into a dedicated `blog.html` index page, with individual blog posts on separate HTML files for better scalability and SEO.

## [1.29.0] - 2024-05-22

### Added
- **Blog Post**: Initial blog post "Why Is My WiFi So Slow in Evanston? A Chicago Tech Expert Explains" moved to a standalone page.
- **Theme Engine**: Persistent Dark/Light mode implementation using `localStorage`.
- **Adaptive Branding**: SVG logo synchronization that updates based on the active theme.
- **WhatsApp Integration**: Added "Scan to Chat" QR code and floating contact action.
- **UI Components**: Implementation of a character counter for the contact form message area.
- **UX**: Responsive vertical timeline for the "How It Works" section on mobile devices.
- **Accessibility**: Added skip-to-content link and improved ARIA labels for modal navigation.

### Changed
- **Form Handling**: Migrated standard POST submission to AJAX-based Formspree integration for a seamless user experience.
- **Performance**: Optimized logo assets with `decoding="async"` and explicit aspect ratios to improve Cumulative Layout Shift (CLS).
- **SEO**: Updated Google Site Verification and Open Graph metadata.

### Fixed
- Resolved an issue where the mobile navigation menu would remain open after a link was clicked.
- Fixed background overlay contrast issues in Light Mode.
- Corrected scroll-margin-top offsets for section anchors to prevent header clipping.

### Removed
- Disabled the experimental AI Chatbot UI pending backend stabilization.

## [1.0.0] - 2024-01-15

### Added
- Initial launch of the MeshCon single-page business website.
- Core services section (PC Repair, WiFi Setup, Smart Home).
- Integrated service area map for Chicago and 35-mile radius.
- Basic contact form via Formspree.
- Responsive grid layout for services and client reviews.
- FAQ section with expandable details.
- Legal and Privacy policy blocks.

---
*Note: Dates follow the YYYY-MM-DD format.*

[Unreleased]: https://github.com/crazykat8091/meshcon/compare/v1.29.0...HEAD
[1.29.0]: https://github.com/crazykat8091/meshcon/compare/v1.0.0...v1.29.0
[1.0.0]: https://github.com/crazykat8091/meshcon/releases/tag/v1.0.0