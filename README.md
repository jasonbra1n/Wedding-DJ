# Wedding DJ Landing Page

A modern, feature-rich landing page template for Wedding DJs.  
Originally created for **DJ Jason Brain (ΙΑΣΩΝ)**, serving Haliburton, Minden, and Kawartha Lakes, Ontario.

> **This project is public, remix-ready, and perfect for other DJs—just fork, personalize, and launch your own site!**

---

## 🎧 [Live Demo](https://weddingdj.jasonbrain.com/)

---

## ✨ Features

### 🎨 Interactive Elements
- **Animated Header Canvas**  
  50 RGB lights orbit the cursor/touch with comet trails and ripple effects on click/tap
- **Dynamic Booking Year**  
  "Booking Now for [current year + 1]" updates automatically
- **Interactive Package Selection**  
  Click any package card to highlight it as the selected option
- **Smooth Scroll Navigation**  
  Animated scroll-to-top button and smooth section transitions

### 📱 Responsive Design
- **Mobile-First Approach**  
  Fully optimized for desktop, tablet, and mobile devices
- **Touch-Friendly Interface**  
  All interactive elements work seamlessly on touch devices
- **Adaptive Layouts**  
  Grid systems automatically adjust for different screen sizes

### 🎵 Audio & Visual Production
- **Multiple Mix Showcases**  
  Three embedded HearThis.at players showcasing different musical styles:
  - Melodic House (cocktail hour vibes)
  - 90s Dancehall (high-energy classics)  
  - Euro Dance (guaranteed dance floor fillers)
- **Visual Production Section**  
  Dedicated section highlighting projection mapping and visual effects capabilities
- **Professional Equipment Showcase**  
  Details on Resolume Arena, UV/blacklight systems, and projection mapping

### 💰 Monetization Features
- **"Fund the Vibes" Section**  
  PayPal integration for tips/donations with emoji-rich, engaging design
- **Tiered Package Pricing**  
  Three clear service tiers: Essential ($2,000), Complete ($2,800), Luxury ($3,500)
- **Visual Production Add-On**  
  Premium upgrade option (+$1,500) for projection mapping services

### 🔍 SEO & Analytics
- **Google Analytics Integration**  
  Full Google Tag Manager and Analytics setup (G-2RTGH4Z617)
- **Google AdSense Ready**  
  AdSense integration for potential revenue streams
- **Rich Schema Markup**  
  LocalBusiness structured data for better search visibility
- **Local SEO Optimization**  
  Targeted keywords for Haliburton, Minden, and Kawartha Lakes

### 📞 Professional Contact System
- **Formspree Integration**  
  Secure contact form with no exposed email addresses
- **Two-Column Contact Layout**  
  Form and interactive Google Maps side-by-side
- **Service Area Details**  
  Clear geographic coverage and travel information

---

## 🚀 Quick Start

1. **Clone the Repository**
    ```bash
    git clone https://github.com/jasonbra1n/Wedding-DJ.git
    cd Wedding-DJ
    ```

2. **Preview Locally**
    ```bash
    # Open index.html in your browser
    # No build tools required—pure HTML, CSS, and JavaScript
    ```

3. **Customize for Your Business**
    - **Content**: Edit `index.html` for your DJ name, services, and packages
    - **Styling**: Modify `styles.css` for colors, fonts, and branding
    - **Interactions**: Adjust `script.js` for animation tweaks
    - **Analytics**: Replace Google Analytics ID with your own
    - **Form**: Update Formspree endpoint for your contact form

4. **Deploy**
    - Host on GitHub Pages, Netlify, Vercel, or any static hosting
    - For custom domains, update the canonical URL in meta tags

---

## 🎨 Customization Guide

### Color Scheme
The site uses a sophisticated purple-to-orange gradient palette:
- Primary: `#291259` (deep purple)
- Secondary: `#8146ff` (vibrant purple)  
- Accent: `#ff6f61` (coral orange)
- Backgrounds: `#f8f4ff` (light purple tint)

### Typography
- Headers: Bold Arial for impact
- Body: Arial for readability
- Special Elements: Italic styling for quotes and emphasis

### Layout Sections
1. **Hero Header** - Animated canvas with call-to-action
2. **About** - Personal story and credentials with image
3. **Audio Samples** - Three mix players showcasing versatility
4. **Visual Production** - Premium service highlighting
5. **Venues** - Supported venue types with images
6. **Gallery** - Past event photography
7. **Blog/FAQ** - Local SEO content
8. **Fund the Vibes** - Tip/donation section
9. **Packages** - Service tier pricing
10. **Contact** - Form and map integration

---

## 🎵 Audio Integration

The site features three HearThis.at embedded players:

```html
<!-- Example: Melodic House Mix -->
<iframe src="https://app.hearthis.at/embed/11056567/..." 
        width="100%" height="150">
</iframe>
```

**To customize:**
1. Upload your mixes to HearThis.at or SoundCloud
2. Get the embed code
3. Replace the iframe `src` attributes
4. Update descriptions and Mixcloud links

---

## 💻 Interactive Header Animation

The canvas animation creates an immersive experience:

```javascript
// 50 RGB lights with orbital motion
for (let i = 0; i < 50; i++) {
  lights.push({
    radius: Math.random() * header.clientWidth,
    angle: Math.random() * Math.PI * 2,
    color: colors[Math.floor(Math.random() * colors.length)],
    trail: []
  });
}
```

**Performance optimization:**
- Reduces particle count on mobile
- Efficient trail rendering
- Smooth 60fps animation

---

## 📊 Analytics & Monetization

### Google Analytics Setup
```html
<script async src="https://www.googletagmanager.com/gtag/js?id=G-2RTGH4Z617"></script>
```

### PayPal Integration
```html
<a href="https://www.paypal.com/paypalme/jasonbrain" 
   class="paypal-button">Fund the Vibes via PayPal</a>
```

### AdSense Ready
```html
<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-0633259514526906"></script>
```

---

## 🛡️ Security & Privacy

- **Formspree Contact Forms**: No server-side code required
- **External Script Loading**: Only from trusted CDNs
- **No Sensitive Data**: All credentials in environment variables
- **HTTPS Ready**: Secure hosting compatible

---

## 📱 Mobile Optimization

- **Touch Gestures**: Full touch support for all interactions
- **Responsive Images**: Automatic scaling and lazy loading
- **Mobile Navigation**: Optimized button sizes and spacing
- **Performance**: Reduced animations on mobile for battery life

---

## 🎯 SEO Features

### Local Business Schema
```json
{
  "@type": "LocalBusiness",
  "name": "Jason Brain Wedding DJ",
  "address": {
    "addressLocality": "Haliburton",
    "addressRegion": "ON"
  }
}
```

### Meta Optimization
- Title: Keyword-rich, location-specific
- Description: Service-focused with local terms
- Keywords: Wedding DJ, location names, services

---

## 🔧 Technical Stack

- **Frontend**: Pure HTML5, CSS3, JavaScript (ES6+)
- **Analytics**: Google Analytics 4, Google Tag Manager
- **Forms**: Formspree for secure submissions
- **Hosting**: Static hosting compatible (GitHub Pages, Netlify, etc.)
- **Maps**: Google Maps embedded iframe
- **Audio**: HearThis.at embedded players

---

## 🚀 Performance

- **Lighthouse Score**: 90+ across all metrics
- **Loading Speed**: Optimized images and lazy loading
- **Core Web Vitals**: Meets Google's performance standards
- **Mobile Performance**: Touch-optimized with reduced animations

---

## 🤝 Contributing

### For Other DJs
1. Fork this repository
2. Customize with your branding and content
3. Deploy to your preferred hosting platform
4. Share your remix in [Discussions](https://github.com/jasonbra1n/Wedding-DJ/discussions)

### Feature Requests
- Open an [Issue](https://github.com/jasonbra1n/Wedding-DJ/issues) for bugs or features
- Submit [Pull Requests](https://github.com/jasonbra1n/Wedding-DJ/pulls) for improvements
- Join [Discussions](https://github.com/jasonbra1n/Wedding-DJ/discussions) for ideas

---

## 📄 License

MIT License — Free to use, remix, and distribute.

**Assets**: Demo images and audio are placeholders—replace with your own content.

---

## 🙏 Credits

**Created by**: [Jason Brain (ΙΑΣΩΝ)](https://jasonbrain.com)  
**Contact**: [jason@weddingdj.jasonbrain.com](mailto:jason@weddingdj.jasonbrain.com)  
**Social**: [@JasonBra1n](https://x.com/JasonBra1n) | [@jason.bra1n](https://www.tiktok.com/@jason.bra1n)

**Special Thanks**:
- DJ Klutch for collaborative mixes
- HearThis.at for audio hosting
- Formspree for secure contact forms

---

## ⭐ Show Your Support

If this template helped launch your DJ business:
- ⭐ Star this repository
- 🔄 Share your customized version
- 💬 Join our [Discussions](https://github.com/jasonbra1n/Wedding-DJ/discussions)
- 🎵 Tag us when you book your first wedding!

---

**Ready to launch your Wedding DJ business? Fork this repo and make it yours!** 🎧✨
