# VOLTEX — Custom Clothing, Printing & Design

Official landing page for **VOLTEX**, a custom clothing, printing, design, and branding studio based in **Sidi Ali Mellal, Tiaret, Algeria**. The page presents VOLTEX's services, process, product range, customer reviews, and contact channels, all inside a single-file, dependency-light, dark-themed website.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Sections](#sections)
- [Technologies](#technologies)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Customization](#customization)
- [Contact Information](#contact-information)
- [Browser Support](#browser-support)
- [License](#license)

## Overview

VOLTEX turns ideas into finished, customized clothing and branded products for individuals, teams, clubs, events, and businesses. This repository contains the public landing page that explains who VOLTEX is, what it does, how the ordering process works, and how visitors can get in touch.

The site is a **static single-page website**. There is no server, no database, and no build step required to run it.

## Features

- Fully responsive layout for desktop, tablet, and mobile.
- Dark theme with a pure-black background and white accent color.
- Smooth scroll navigation and mobile menu with integrated social icons.
- Animated page reveals powered by AOS (Animate On Scroll).
- Horizontal, infinite-looping review marquee (pauses on hover).
- Clickable product images with a built-in lightbox viewer.
- Contact section with the studio's address, phone, email, and 24/7 availability.
- Social media links for Instagram, Facebook, TikTok, WhatsApp, and Telegram.
- Accessible markup: semantic tags, ARIA labels, keyboard-friendly interactions, and alt text.

## Sections

The page is divided into the following sections, reachable from the top navigation:

| Section | Description |
| --- | --- |
| Hero | Headline, subheading, and call-to-action buttons with a showcase photo. |
| Services | Cards describing custom clothing, design, printing, and branding services. |
| How It Works | Horizontal timeline of the 5-step ordering process (Share, Design, Customize, Quality Check, Receive). |
| For Individuals | Personalization offer for individual customers with a product photo. |
| Products | Four product images (T-shirts, custom apparel, branded clothing, streetwear) with click-to-zoom lightbox. |
| About | Reasons to choose VOLTEX. |
| Reviews | Customer feedback shown as an infinite horizontal scrolling marquee. |
| Social Media | Follow-us cards linking to the studio's social profiles. |
| Contact | Request-a-quote form plus address, phone, email, and availability details. |
| Footer | Brand, navigation, services, social links, and contact information. |

## Technologies

- **HTML5** — semantic page structure
- **CSS3** — custom design system and responsive styling
- **Bootstrap 5.3.8** — layout grid and UI components (via CDN)
- **Bootstrap Icons 1.13.1** — icon set (via CDN)
- **AOS (Animate On Scroll)** — scroll-triggered animations (via CDN)
- **Google Fonts** — Inter, Lexend, Source Code Pro
- **Vanilla JavaScript** — smooth scrolling, lightbox, back-to-top, and small interactions

All external libraries are loaded from public CDNs; the project itself runs without a package manager or bundler.

## Project Structure

```
landing-consulting/
├── landing-consulting.html      # Entire website (markup, styles, scripts)
├── README.md                    # This file
└── assets/
    ├── css/
    │   └── bootstrap-theme.css  # Custom Bootstrap theme overrides
    ├── img/
    │   ├── white.png            # White V logo mark (navbar, footer)
    │   ├── name.png             # VOLTEX wordmark
    │   ├── black.png            # Black V logo mark (alternate)
    │   ├── 3.png                # For Individuals section photo
    │   ├── salim back.png       # Hero showcase photo
    │   └── cust/                # Product photos
    │       ├── Choose Yourself Oversize T-Shirt Modern Streetwear.jpeg
    │       ├── Unisex T Shirt.jpeg
    │       ├── URBAN Oversized Unisex Streetwear Tee _ Japanese Rooftop Style.jpeg
    │       └── Black Oversized Heavyweight T-Shirt _ Premium Unisex Graphic Tee.jpeg
    └── js/
        └── bootstrap.bundle.js  # Placeholder (the page uses the Bootstrap CDN bundle)
```

**Note:** `assets/js/bootstrap.bundle.js` is only a placeholder and is not referenced by the page. Bootstrap is loaded from the CDN at the bottom of `landing-consulting.html`.

## Getting Started

Because this is a static page, no installation or build step is required.

1. Clone or download the repository.
2. Make sure the `assets/` folder stays in the same directory as `landing-consulting.html` (all image and style paths are relative).
3. Open `landing-consulting.html` in a web browser.

The page will also run correctly on a simple static file server:

```bash
python3 -m http.server 8000
```

Then open `http://localhost:8000` in your browser.

## Customization

### Business information

All contact details live in the **Contact** section and the **Footer** of `landing-consulting.html`:

- Address: Sidi Ali Mellal, Tiaret, Algeria
- Phone / WhatsApp: 0558340669
- Email: voltex.tiaret@gmail.com
- Availability: 24/24, 7/7

### Social media links

Social links appear in three places, each of which should be updated together:

- **Desktop navbar** — shown in the mobile dropdown menu on small screens
- **Social media section** — colored cards (black-and-white style)
- **Footer** — round icon buttons

Current profiles:

- Instagram: https://www.instagram.com/vol_tex7
- Facebook: https://www.facebook.com/profile.php?id=61593866157599
- TikTok: https://www.tiktok.com/@vol_tex7
- WhatsApp: https://wa.me/213558340669 (uses the studio phone number)
- Telegram: https://t.me/aziz_benallou

### Product images

Product photos live in `assets/img/cust/`. To add, remove, or replace products, edit the four product cards in the **Products** section and place new images in that folder.

### Reviews

The reviews shown in the marquee are sample/placeholder feedback. Replace the text, names, and initials in the review cards with real customer reviews when available.

### Theme

The color system is defined once at the top of the `<style>` block in `landing-consulting.html` under `:root`. To restyle the site, adjust the CSS custom properties there (for example `--vx-bg` and `--vx-purple-bright`).

## Contact Information

- **Address:** Sidi Ali Mellal, Tiaret, Algeria
- **Phone / WhatsApp:** 0558340669
- **Email:** voltex.tiaret@gmail.com
- **Availability:** 24 hours a day, 7 days a week

## Browser Support

The site targets current versions of Chrome, Firefox, Safari, and Edge. Older browsers may not fully support modern CSS features used by the design system.

## License

This project is a private business website for VOLTEX. All branding, logo assets, and photographs are property of VOLTEX. External libraries (Bootstrap, Bootstrap Icons, AOS, and Google Fonts) are used under their respective licenses.