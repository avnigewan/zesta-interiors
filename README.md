# Zesta Interiors

A modern, responsive marketing website for **Zesta Interiors**, an end-to-end home interior design company. Built as a static site and hosted on GitHub Pages.

**Live site:** https://avnigewan.github.io/zesta-interiors/

Tagline: *Design that delights.*

## Overview

Zesta Interiors is a HomeLane-style interior design brand. The site presents the company's services, portfolio, pricing and a lead-capture contact experience, with a clean, contemporary look built on a warm terracotta accent palette.

## Pages

| Page | File | Purpose |
| --- | --- | --- |
| Home | `index.html` | Hero, key stats, service highlights and testimonials |
| About | `about.html` | Company story and approach |
| Services | `services.html` | Full-home design, kitchens, wardrobes and more |
| Portfolio | `portfolio.html` | Showcase of project imagery |
| Pricing | `pricing.html` | Package tiers with a featured plan |
| Contact | `contact.html` | Lead form, FAQ accordion, business hours, map and WhatsApp |

## Features

- Modern design system using the Fraunces and Inter typefaces
- Glassy sticky header with an SVG house logo mark
- Consistent footer with social links across every page
- Mobile hamburger navigation (pure CSS, no JavaScript)
- Contact page with an FAQ accordion, business hours and a mailto link
- Embedded Google Map on the contact page
- Site-wide floating WhatsApp click-to-chat button
- Custom SVG favicon
- Fully responsive layout with subtle entrance animations

## Design tokens

| Token | Value |
| --- | --- |
| Brand accent | `#e6733a` |
| Brand gradient | `#f0954a` to `#c9551f` |
| Ink / text | `#2a2622` |
| Background | `#faf6f1` |
| Corner radius | `18px` |

## Tech stack

- Plain HTML5 and CSS3 (single `style.css`)
- No build step, no frameworks, no dependencies
- Google Fonts for typography
- Hosted on GitHub Pages

## Project structure

```
zesta-interiors/
├── index.html
├── about.html
├── services.html
├── portfolio.html
├── pricing.html
├── contact.html
├── style.css
├── favicon.svg
└── README.md
```

## Local development

No tooling is required. Clone the repository and open `index.html` in a browser, or serve the folder with any static file server:

```bash
# Python 3
python -m http.server 8000

# then open http://localhost:8000
```

## Configuration to complete

A few items use placeholders and should be updated with real business details:

1. **WhatsApp number** — every WhatsApp link points to `https://wa.me/91XXXXXXXXXX`. Replace `91XXXXXXXXXX` with the real number in international format (country code + number, no `+` or spaces).
2. **Contact form delivery** — the form currently shows a thank-you message only. Connect it to a form backend (for example a Formspree endpoint) and add `name` attributes to the fields to receive leads.
3. **Contact details** — the email (`hello@zestainteriors.com`), phone and office locations are placeholders and should be replaced with real ones.
4. **Project photos** — the portfolio currently uses stock imagery; swap in real project photos when available.

## Deployment

The site is deployed via **GitHub Pages** from the `main` branch. Any commit to `main` is published automatically at the live URL above.

## License

© 2026 Zesta Interiors. All rights reserved.
