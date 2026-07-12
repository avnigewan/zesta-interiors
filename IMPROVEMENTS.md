# Zesta Interiors — Website Improvement Suggestions

A review of the current site (https://avnigewan.github.io/zesta-interiors/) benchmarked against leading interior-design sites (Livspace, HomeLane, Design Cafe). Items are ordered by impact.

## Priority 1 — Lead capture (highest business impact)

The site currently captures no leads. Both primary forms fail to submit:

- **Contact "Book Your Free Consultation" form** — has no backend. It only shows a client-side "Thank you!" message and does not send the enquiry anywhere. Fields also lack `name` attributes.
- **Vastu "Analyse My Home" form** — uses `onsubmit="return false"`, so it never submits or produces output.
- **WhatsApp links** — every "Chat on WhatsApp" button still points to the placeholder `wa.me/91XXXXXXXXXX`.

**Actions**
- Connect both forms to a backend (e.g. Formspree) and add `name` attributes to all fields.
- Replace the placeholder WhatsApp number with the real number in international format.
- Make the Vastu tool actually generate room-by-room guidance output.

## Priority 2 — SEO & shareability

None of the pages include a meta description or Open Graph tags. This causes poor Google snippets and blank link previews on WhatsApp/Instagram.

**Actions**
- Add a unique `<meta name="description">` per page.
- Add Open Graph tags: `og:title`, `og:description`, `og:image`, `og:url`.
- Add a `sitemap.xml` and structured data (LocalBusiness + Review schema).

## Priority 3 — Portfolio & imagery

The portfolio uses stock photography with no `alt` attributes; the contact page also uses stock images.

**Actions**
- Swap in real Zesta project photos, ideally with before/after comparisons.
- Add descriptive `alt` text to every image (accessibility + SEO).
- Give each project a short case study: city, home size, budget range, style.
- Add filtering by room or style.

## Priority 4 — Trust signals

Testimonials are text-only with generic names.

**Actions**
- Add client or project photos to testimonials.
- Link to Google / Houzz review profiles.
- Add brand / material partner logos (e.g. Hettich, Ebco, Century).
- Add named designer bios on the About page.
- Surface press mentions or awards if available.

## Priority 5 — UX & conversion polish

**Actions**
- Add a cost estimator / "instant ballpark" calculator alongside the pricing tiers.
- Add a sticky mobile call / WhatsApp bar.
- Lazy-load images and compress assets for faster load.
- Add a favicon-based social preview image.

## What already works well (keep)

- Fast, dependency-free build with a single stylesheet — easy to maintain.
- Clear four-step process (Consult -> Design -> Build -> Move In).
- Transparent, published pricing tiers (many competitors hide this).
- FAQ accordion on the homepage.
- Vastu Sense — a genuine differentiator few competitors offer.

---

_Generated as a planning reference. No functional code changes are included in this document._
