# Quran Kareem Website Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Create a modern, Apple-inspired website for the Quran Kareem app with landing page, Privacy Policy, Terms of Use (Solana dApp Store Publisher Policy compliant), and official assets.

**Architecture:** Vanilla HTML5, CSS3, and JavaScript using Apple Design Tokens from `Design.md`. Clean semantic HTML5, glassmorphic headers, responsive CSS, and interactive screenshot gallery.

**Tech Stack:** HTML5, Vanilla CSS3 (custom properties), Vanilla JavaScript ES6+.

## Global Constraints

- Design system tokens strictly follow `Design.md` (Apple Blue `#0071e3`, Inter typography, light/dark binary section pacing, pill CTAs `980px` radius).
- Privacy Policy & Terms of Use must satisfy **Solana Mobile dApp Store Publisher Policy**.
- All assets (logo, 9 screenshots) copied from `C:\Users\PopGore\.gemini\antigravity-ide\scratch\Quran` to `website quran/assets/`.

---

### Task 1: Asset Preparation & Project Setup

**Files:**
- Create: `assets/logo.webp`
- Create: `assets/screenshots/screenshot_1.png` .. `screenshot_9.png`
- Create: `css/style.css`

**Interfaces:**
- Produces: CSS design system tokens and image assets for HTML pages.

- [ ] **Step 1: Create directories for CSS, JS, and Assets**

```bash
mkdir -p css js assets/screenshots
```

- [ ] **Step 2: Copy official logo and screenshots from Quran app repository**

Copy `icon_launcher_round.webp` to `assets/logo.webp` and `fastlane/metadata/android/en-US/images/phoneScreenshots/Screenshot_1.png..9.png` to `assets/screenshots/`.

- [ ] **Step 3: Create `css/style.css` with Design.md tokens**

Define `:root` CSS variables for colors, typography, spacing, elevation, border-radii, glassmorphism, responsive grid layout, and dark/light section styles.

- [ ] **Step 4: Commit setup task**

```bash
git add css/style.css assets/
git commit -m "feat: initialize design tokens and asset structure for Quran Kareem website"
```

---

### Task 2: Build Landing Page (`index.html`) & Interactive JS (`js/main.js`)

**Files:**
- Create: `index.html`
- Create: `js/main.js`

**Interfaces:**
- Consumes: Design system tokens in `css/style.css`, image assets in `assets/`.
- Produces: Primary landing page with glass navbar, dark hero, light features grid, screenshot carousel/showcase, download section, and footer.

- [ ] **Step 1: Write `js/main.js`**

Implement smooth scroll, active navigation highlights, dynamic screenshot modal/lightbox, and interactive theme toggling.

- [ ] **Step 2: Write `index.html`**

Create semantic HTML5 structure:
- `<header class="glass-nav">`: Logo, brand name "Quran Kareem", menu links, and "Download App" CTA.
- `<section class="hero-dark">`: Headline, tagline, pill CTAs, interactive device mockup displaying app screenshots.
- `<section class="features-light">`: 6 feature card highlights (No Ads, Tafsir & Translation, Audio Recitations, Mushaf Mode, Reminders & Notes, Verse Search).
- `<section class="screenshots-dark">`: Interactive screenshot showcase slider with 9 app screenshots.
- `<section class="download-light">`: Download buttons (Solana dApp Store APK, Google Play, IzzyOnDroid, GitHub Release).
- `<footer class="footer-dark">`: Quick links, license info (GPLv3), and social links.

- [ ] **Step 3: Commit landing page task**

```bash
git add index.html js/main.js
git commit -m "feat: create landing page index.html and main.js for Quran Kareem website"
```

---

### Task 3: Build Privacy Policy Page (`privacy.html`)

**Files:**
- Create: `privacy.html`

**Interfaces:**
- Consumes: Design system tokens in `css/style.css`.
- Produces: Solana Mobile dApp Store Publisher Policy compliant Privacy Policy document.

- [ ] **Step 1: Write `privacy.html`**

Create structured Privacy Policy covering:
- Zero Personal Data Collection Notice (no analytics, no GPS, no device IDs).
- Local Data Storage (notes, bookmarks, settings remain on device).
- Network Requests & Audio Servers (QuranEnc, EveryAyah, Tarteel audio fetching).
- User Rights under Open Source GPLv3.
- Compliance with Solana Mobile Publisher Policy & contact details.

- [ ] **Step 2: Commit Privacy Policy task**

```bash
git add privacy.html
git commit -m "feat: create Solana Mobile compliant Privacy Policy page"
```

---

### Task 4: Build Terms of Use Page (`terms.html`)

**Files:**
- Create: `terms.html`

**Interfaces:**
- Consumes: Design system tokens in `css/style.css`.
- Produces: Solana Mobile dApp Store Publisher Policy compliant Terms of Use document.

- [ ] **Step 1: Write `terms.html`**

Create structured Terms of Use covering:
- Agreement to Terms & App Usage Guidelines.
- Intellectual Property Rights (Holy Qur'an text attribution, open-source code GPLv3).
- No Warranty & Limitation of Liability (standard dApp store requirement).
- Governing Policy & Contact Info (`concerns@dappstore.solanamobile.com` / GitHub issues).

- [ ] **Step 2: Commit Terms of Use task**

```bash
git add terms.html
git commit -m "feat: create Solana Mobile compliant Terms of Use page"
```

---

### Task 5: Verification & Quality Assurance

**Files:**
- Audit all HTML, CSS, JS files and links across `index.html`, `privacy.html`, `terms.html`.

- [ ] **Step 1: Verify all internal link routes and glassmorphism styling**
- [ ] **Step 2: Verify responsive design on mobile and desktop viewports**
- [ ] **Step 3: Check Solana dApp Store Policy compliance across both policy documents**
