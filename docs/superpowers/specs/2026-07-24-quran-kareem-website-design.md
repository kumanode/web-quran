# Design Spec: Quran Kareem App Website

## Overview
A modern, Apple-inspired website for the **Quran Kareem** mobile application built with Vanilla HTML5, CSS3, and JavaScript. The site incorporates the design tokens and principles from `Design.md` (Apple Blue `#0071e3`, crisp typography, binary light/dark contrast pacing, glassmorphism nav), features official app assets/logo, and includes Privacy Policy and Terms of Use documents compliant with the **Solana Mobile dApp Store Publisher Policy**.

---

## 1. Design System & Aesthetics (per Design.md)

### Color Palette
- **Primary / CTA Accent**: `#0071e3` (Apple Blue) / `#2997ff` (Dark mode accent)
- **Backgrounds**:
  - Dark Cinematic Sections: `#000000` (Pure Black) with `#ffffff` text
  - Light Open Sections: `#f5f5f7` (Apple Light Gray) / `#ffffff` (Pure White) with `#1d1d1f` text
  - Elevated Cards: `#f5f5f7` (Light) / `#1d1d1f` (Dark)
- **Navigation**: Glassmorphism backdrop filter (`backdrop-filter: blur(20px)`, `rgba(0,0,0,0.8)` or `rgba(255,255,255,0.8)`)

### Typography & Layout
- **Font Stack**: `"Inter", -apple-system, BlinkMacSystemFont, "SF Pro Display", sans-serif`
- **Headings**: Display Hero 56px (font-weight 600, negative letter-spacing `-0.015em`), Section Title 40px (600), Tile Heading 28px.
- **Buttons**: Pill-shaped CTAs (border-radius `980px`), no heavy drop shadows, border-free cards with soft hover elevation.

---

## 2. Website Architecture & File Structure

Target Directory: `c:\Users\PopGore\.gemini\antigravity-ide\scratch\website quran`

```
c:\Users\PopGore\.gemini\antigravity-ide\scratch\website quran/
├── index.html           # Main Landing Page with hero, features, showcase, download section
├── privacy.html         # Solana Mobile dApp Store Publisher Policy compliant Privacy Policy
├── terms.html           # Solana Mobile dApp Store Publisher Policy compliant Terms of Use
├── css/
│   └── style.css        # Pure Vanilla CSS design tokens & responsive components
├── js/
│   └── main.js          # Interactive features (screenshot gallery, modal, theme switch, smooth scroll)
└── assets/
    ├── logo.webp        # Official app launcher logo
    └── screenshots/     # Official high-res screenshots 1-9
```

---

## 3. Page Structure & Features

### 3.1 Main Landing Page (`index.html`)
1. **Header / Navbar**:
   - Fixed translucent glass navbar with logo, "Quran Kareem" brand title, links to Features, Screenshots, Privacy Policy, Terms of Use, and a prominent "Download App" CTA.
2. **Hero Section (Cinematic Black `#000000`)**:
   - Headline: *"Read, Explore, and Reflect on the Holy Qur’an"*
   - Tagline: *"Quran Kareem — Ad-free, 100% privacy-focused, and open source."*
   - Interactive Device Mockup showcasing active app screenshots.
   - Primary Pill CTAs: "Download APK / Solana dApp Store" & "Explore Features".
3. **Key Highlights Grid (`#f5f5f7`)**:
   - 🚫 **Zero Ads & Zero Tracking**: Built with complete privacy in mind (no GPS, no camera, no analytics).
   - 📙 **Tafsirs & Translations**: Multi-language translations with classical tafsirs side-by-side.
   - 🎙️ **Audio Recitations**: High quality recitations with synced ayah highlighting.
   - 📄 **Mushaf Mode**: Authentic page layout experience with custom Arabic typography.
   - ❤️ **Verse Reminders & Notes**: Personal reflection tools stored safely offline on your device.
4. **App Screenshots Showcase (`#000000`)**:
   - Interactive slider / grid showcasing 9 phone screenshots from the app.
5. **Solana dApp Store & Download Section (`#ffffff`)**:
   - Download options: Solana Mobile dApp Store APK, Google Play, IzzyOnDroid, GitHub Release.
6. **Footer (`#1d1d1f`)**:
   - Navigation links, Community links (Discord, Matrix, Telegram), Copyright, and GPLv3 Open Source badge.

### 3.2 Privacy Policy (`privacy.html`)
Fully formatted document satisfying Solana Mobile dApp Store Publisher Policy:
- **Zero Data Collection**: Explicitly states no personal information, analytics, location, or telemetry is gathered.
- **On-Device Storage**: Bookmarks, notes, and settings remain 100% local.
- **Third-Party Services**: Audio download servers (QuranEnc, EveryAyah, Tarteel) and audio streaming parameters.
- **User Rights & Open Source**: Complete code transparency under GNU General Public License v3 (GPLv3).

### 3.3 Terms of Use (`terms.html`)
Fully formatted document satisfying Solana Mobile dApp Store Publisher Policy:
- **Acceptance of Terms**: Usage guidelines for Quran Kareem.
- **Intellectual Property & Open Source**: Teks Al-Qur'an source attributions and GPLv3 licensing terms.
- **Disclaimer of Warranties & Limitation of Liability**: Standard app publisher protection terms required by dApp store policies.
- **Governing Policy & Contact**: Direct developer contact details.

---

## 4. Verification & Quality Assurance Plan
1. **Design System Accuracy**: Verify Apple Blue `#0071e3` usage, Inter font loading, pill button radius (`980px`), and dark/light binary pacing.
2. **Asset Integrity**: Ensure `logo.webp` and screenshot assets render cleanly across mobile and desktop viewpoints.
3. **dApp Store Compliance**: Cross-check Privacy Policy and Terms of Use against Solana Mobile Publisher Policy rules.
4. **Browser Verification**: Test responsiveness, glassmorphic headers, and link routing across screen sizes.
