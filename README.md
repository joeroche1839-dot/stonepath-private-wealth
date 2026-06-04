# StonePath Private Wealth Management — Website

A modern, premium, fully responsive marketing website for **StonePath Private Wealth Management** — an independent financial advisory practice led by **David Roche**, serving Peterborough & the Kawarthas, Ontario.

Built by **Digital FrameWorks** as a static site — pure HTML, CSS and vanilla JavaScript. No build step, no dependencies, deploys anywhere.

## Pages

| File | Purpose |
|------|---------|
| `index.html` | Home — hero, services, advisor intro, approach, testimonials, CTA |
| `services.html` | Six core services in detail (wealth, retirement, investment, estate, tax, insurance) |
| `about.html` | David Roche's story (NHL → wealth management), principles, FAQ |
| `approach.html` | The 4-step process + investment philosophy |
| `contact.html` | Contact details + consultation request form |

## Brand & design

- **Identity** — a distinct private-wealth aesthetic: deep navy + refined gold + warm stone, elegant **Playfair Display** headings with **Inter** body, and a "StonePath" cairn (stacked-stones) logo motif. Conservative, trustworthy and premium.
- **Photo-light by design.** This client had **no existing website and no photography**, so the site is intentionally built without stock imagery — its polish comes from typography, color, the navy "stone path" hero treatment and iconography. See *Adding imagery* below.
- **Mobile-first & responsive**; **SEO-ready** (unique meta/OG, canonicals, `sitemap.xml`, `robots.txt`, JSON-LD `FinancialService` schema); **accessible** (ARIA, keyboard nav/FAQ, reduced-motion, strong contrast); **fast** (no frameworks, minimal JS).

## Content & accuracy

Copy is grounded in verified, public facts about **David Roche** (from his Wikipedia profile): Lindsay, ON native; NHL career with Pittsburgh, Calgary and the NY Islanders (drafted 1993); Calder Cup champion; now based in Ennismore and working as a financial advisor in the Peterborough area. Contact: **705-344-7534**, **joeroche1839@gmail.com**.

> No specific licenses, designations, dealer/firm affiliations or performance figures were invented — service descriptions are deliberately general.

## ⚠️ Before publishing — compliance & accuracy (important for a financial site)

- **Regulatory disclosures:** a placeholder disclaimer sits at the bottom of every page. Replace the bracketed text with StonePath's real registration/licensing details, dealer or MGA affiliations, and any mandated disclosures **before going live**.
- **Advisor headshot:** the About page and homepage use a tasteful "DR" monogram where a photo would go. Drop in a professional headshot of David (and optionally a Kawarthas/office photo for the hero) when available.
- **Testimonials** are representative placeholders — replace with real, permissioned client reviews (and confirm testimonial rules for your registration category).
- **Domain:** pages reference `stonepathwealth.ca` as a sample canonical — update to the real domain once chosen.

## Adding imagery later

The CSS is photo-ready: set a hero image by adding `background-image` to `.hero`, swap the About monogram/panel for an `<img>`, and the existing components (split, cards) accept photos with no structural changes.

## Customization checklist

- **Contact form** — `js/main.js` confirms locally as a demo. To receive real submissions, add an `action` URL to `#quote-form` (e.g. `action="https://formspree.io/f/XXXX"`); route it to `joeroche1839@gmail.com`.
- **Fonts/colors** — re-theme via the `:root` block in `css/styles.css`.

## Deployment

Static site — host on Vercel, Netlify, Cloudflare Pages or any host over **HTTPS**. Includes `vercel.json` (security headers).

### Local preview

```bash
cd stonepath-private-wealth
python3 -m http.server 8094
# open http://localhost:8094
```
