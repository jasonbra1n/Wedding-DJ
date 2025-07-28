# Wedding DJ Landing Page

A modern, customizable landing page template for Wedding DJs.  
Originally created for **DJ Jason Brain (ΙΑΣΩΝ)**, serving Haliburton, Minden, and Kawartha Lakes, Ontario.

> **This project is public, remix-ready, and perfect for other DJs—just fork, personalize, and launch your own site!**

---

## 🎧 [Live Demo](https://weddingdj.jasonbrain.com/)

---

## ✨ Features

- **Interactive Animated Header**:  
  - 50 RGB lights orbit the cursor (desktop) or touch point (mobile), with comet-like trails brightest at the head, fading backward.
  - Click/tap to trigger bold, water-like ripples (initial opacity 0.7, max radius full viewport height).
  - Dynamic header text: "Booking Now for [current year + 1]" (e.g., 2026 in 2025).
- **Fully Responsive**:  
  Optimized for desktop, tablet, and mobile with smooth animations and adaptive layouts.
- **SEO Optimized**:  
  Includes meta tags for description and keywords to boost search engine visibility.
- **Easy Customization**:  
  Edit DJ name, region, contact info, images, and colors directly in `index.html`.
- **Modern Visuals**:  
  Gradient backgrounds, glowing call-to-action buttons, smooth scroll-to-top functionality, and vibrant venue/event galleries.
- **Audio Integration**:  
  Embedded HearThis.at player for sample mixes, with a Mixcloud link option.
- **Fork & Remix**:  
  Designed for DJs to adapt for their own business, region, or style.

---

## 🚀 Quick Start

1. **Clone the Repository**:
   ```sh
   git clone https://github.com/jasonbra1n/weddingdj.git
   ```
2. **Open `index.html` Locally**:
   - Open `index.html` in a browser to preview the site.
   - No build tools required—pure HTML, CSS, and JavaScript.
3. **Customize for Your DJ Business**:
   - Edit `index.html` to update:
     - DJ name (line ~110, `<h2>About Jason Brain</h2>`).
     - Region and contact info (lines ~157–160, Contact section).
     - Meta tags for SEO (lines ~7–9).
   - Replace images in the `images/` folder (JPEG/PNG, recommended 1200x800px for header, 300x200px for galleries).
   - Swap the HearThis.at iframe (line ~126) for a Mixcloud embed or remove it.
4. **Deploy Your Site**:
   - Host on GitHub Pages, Netlify, or any static hosting service.
   - Example for GitHub Pages:
     - Push to a `gh-pages` branch or enable Pages in repo settings.
     - Set the custom domain (e.g., `yourdomain.com`) if desired.

---

## 🌀 Interactive Header Animation

The header uses a JavaScript Canvas animation for a mesmerizing effect:
- **50 RGB Lights**: Orbit the cursor/touch point with comet-like trails (10 positions, brightest at the head).
- **Ripples**: Click/tap to create expanding, fading ripples (opacity 0.7 to 0, max radius ~100vh).
- **Dynamic Year**: Header updates to "Booking Now for [current year + 1]" automatically.
- **Performance**: Optimized for smooth rendering, with `mix-blend-mode: overlay` for vibrant colors.

**Customize the animation** in the `<script>` block (~lines 210–300):
- Change light count: Adjust `for (let i = 0; i < 50; i++)` (e.g., to 30 for better performance).
- Modify ripple opacity: Set `opacity: 0.7` in `mousedown`/`touchstart` listeners.
- Adjust trail length: Change `light.trail.length > 10` to 5 or 15.
- Remove animation: Delete the `<canvas class="lights">` and `<script>` block for a static header.

---

## 📸 Content Overview

- **About Section**: Highlight your DJ experience, style, and services (edit ~line 110).
- **Venue Gallery**: Showcase venue types (tents, barns, backyards, halls) with hover effects (~lines 135–148).
- **Event Gallery**: Display past gigs with vibrant images (~lines 150–154).
- **Audio Player**: Embed sample mixes via HearThis.at or Mixcloud (~line 126).
- **Contact & Booking**: Easy-to-edit contact details with email and phone links (~lines 157–160).
- **Scroll-to-Top Button**: Appears on scroll, smoothly returns to the top (~line 168).

---

## 🔀 For Other DJs

This template is built for you to remix!  
Fork the repo, swap in your details, and launch your own Wedding DJ landing page.

- **Keep the Hypnotic Header**: Retain the `<script>` and tweak colors, light count, or ripple effects.
- **Go Minimal**: Remove the `<canvas>` and `<script>` for a clean, static look.
- **Add Your Flair**: Update fonts, colors (e.g., `.cta-button` background `#ff6f61`), or add new sections.

---

## 🛠️ Troubleshooting

- **Animation Lag**: Reduce lights (`i < 50` to `i < 30`) or ripples (`ripples.length > 5` in `<script>`).
- **Images Not Loading**: Ensure images are in the `images/` folder and paths match in `index.html`.
- **Button Issues**: Verify CTA button (`z-index: 1`, `pointer-events: auto`) isn’t blocked by ripples. Add `if (!event.target.closest('.cta-button'))` to `mousedown`/`touchstart` listeners if needed.
- **Mobile Touch Issues**: Check `event.preventDefault()` in `touchmove`/`touchstart` doesn’t interfere with scrolling. Adjust if necessary.

Open a [GitHub Issue](https://github.com/jasonbra1n/weddingdj/issues) for help!

---

## 📄 License

MIT License — Free to use, remix, and share.  
**Note**: Placeholder images in `images/` are for demo purposes and not included in the license. Replace with your own images.

---

## 👋 Credits & Contributions

Created by [Jason Brain (ΙΑΣΩΝ)](https://jasonbrain.com).  
Contact: [jason@weddingdj.jasonbrain.com](mailto:jason@weddingdj.jasonbrain.com).

**Love this template?**  
- Share your remix in [Discussions](https://github.com/jasonbra1n/weddingdj/discussions)!
- Contribute ideas or improvements via [Pull Requests](https://github.com/jasonbra1n/weddingdj/pulls).
- Star the repo to show some love! ⭐

---
