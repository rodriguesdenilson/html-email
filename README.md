# Email Templates

A portfolio of **21 responsive, production-ready HTML email templates** built for cross-client compatibility. Each template represents a distinct brand and use case — from product launches to seasonal sales — demonstrating a range of email development techniques and layout patterns.

> **Note:** The templates do not include real images — the focus is entirely on HTML/CSS structure, layout, responsiveness, and cross-client compatibility. Image placeholders can be swapped for production assets before deployment.

---

## Templates

| # | File | Brand / Theme | Layout Highlights |
|---|------|---------------|-------------------|
| 1 | `project-1-responsive.html` | HTML Email Newsletter | 3-column feature grid, social icons, dark mode |
| 2 | `project-2-responsive.html` | Bomb Nutrition — Halloween Promo | Multi-CTA promotional, orange/dark theme |
| 3 | `project-3-responsive.html` | Hims — Healthcare | Product cards, category sections |
| 4 | `project-4-responsive.html` | Starbucks Rewards | Rewards table, green brand palette |
| 5 | `project-5-responsive.html` | Malibu Rum — Tropical Boo Bash | Cocktail recipes, gradient backgrounds |
| 6 | `project-6-responsive.html` | Oobli — Halloween Sale | Discount promo, lime/orange palette |
| 7 | `project-7-responsive.html` | Fleet Feet — Milestones | Birthday gift offer, navy/gold theme |
| 8 | `project-8-responsive.html` | Confused.com — App Download | 6-section feature showcase, dark theme |
| 9 | `project-9-responsive.html` | MINI — Motortober Rally | Automotive event, financing offers |
| 10 | `project-10-responsive.html` | Rest Bedding — Summer Sale | Product showcase, comparison table |
| 11 | `project-11-responsive.html` | Plaid — Lending Tools Launch | Hero + partner logos, side-by-side content, teal/navy palette |
| 12 | `project-12-responsive.html` | Calendly — Workflows Feature | Feature checklist, milestone badge, blue brand palette |
| 13 | `project-13-responsive.html` | Plaid — AI Tools Launch | Chat mockup, AI provider diagram, testimonial, dark navy/cyan |
| 14 | `project-14-responsive.html` | DIME Beauty — Anniversary Sale | Top-10 product grid, numbered badges, gold/charcoal theme |
| 15 | `project-15-responsive.html` | Gainful — 7th Birthday Giveaway | Hero product shot, minimal layout, beige/neutral palette |
| 16 | `project-16-responsive.html` | TALEA Beer Co. — 1st Anniversary | Alternating image/text, taproom section, coral/sandy palette |
| 17 | `project-17-responsive.html` | A Book Apart — Spring Sale | Discount badge, book list, red/coral accent |
| 18 | `project-18-responsive.html` | Methodical — Japanese Green Tea | Product launch hero, shop-by-category grid, sage/tan palette |
| 19 | `project-19-responsive.html` | SHIFT Robotics — Black Friday | Product hero, social icon row, black/neon-yellow theme |
| 20 | `project-20-responsive.html` | Ocean Supplements — Black Friday | Pricing tiers, benefit cards, testimonials, trust badges |
| 21 | `project-21-responsive.html` | 1906 Wellness — Black Friday Sale | Typographic "SALE" hero, product section, purple/yellow palette |

---

## Features

- **Responsive design** — adapts from desktop to mobile via `@media (max-width: 600px)` breakpoints
- **Dark mode support** — uses `prefers-color-scheme` media query and CSS custom properties
- **Outlook compatibility** — VML fallbacks, conditional comments (`<!--[if mso]>`), and MSO-specific resets
- **Bulletproof buttons** — dual-layer approach combining VML (Outlook) and HTML/CSS anchors
- **Accessibility** — ARIA roles, descriptive `alt` attributes, semantic headings, and sufficient color contrast
- **No external dependencies** — all styles are inline or scoped; no JavaScript, no web fonts required
- **UTM tracking** — CTA links include `utm_source`, `utm_medium`, `utm_campaign`, and `utm_content` parameters

---

## Technical Details

### Compatibility
| Client | Support |
|--------|---------|
| Outlook 2013–365 | Full (VML + conditional comments) |
| Apple Mail / iOS Mail | Full |
| Gmail | Full |
| Outlook.com / Hotmail | Full |
| Yahoo Mail | Full |
| Samsung Mail | Full |

### Layout & Styling
- **Layout engine:** HTML tables (required by email clients; CSS Grid and Flexbox are not supported)
- **Inline styles:** Primary styling method to survive email client CSS stripping
- **Media queries:** Used exclusively for responsive behavior and dark mode — not stripped by modern clients
- **Font stacks:** System-safe fallbacks (`Arial, Helvetica, sans-serif`) — no reliance on web fonts

<details>
<summary>Mobile Classes</summary>

| Class | Purpose |
|-------|---------|
| `.email-container` | Forces full width on mobile |
| `.stack-column` | Converts multi-column to single column |
| `.mobile-padding` | Adjusts spacing for small screens |
| `.mobile-img` | Resizes images for mobile |
| `.mobile-hide` | Hides elements on mobile |
| `.mobile-only` | Shows elements only on mobile |

</details>

<details>
<summary>Dark Mode</summary>

Supported via `<meta name="color-scheme" content="light dark">` and CSS variables in `:root`.

```css
@media (prefers-color-scheme: dark) {
  .dark-mode-bg   { background-color: #1a1a1a !important; }
  .dark-mode-text { color: #e0e0e0 !important; }
}
```

</details>

---

## Usage

1. Open any `.html` file directly in a browser for a quick preview — each template is self-contained, no build steps required.
2. To test across email clients, paste the HTML into a tool such as [Litmus](https://litmus.com) or [Email on Acid](https://www.emailonacid.com).
3. Replace placeholder image URLs (e.g., `ibb.co`, `via.placeholder.com`) with your own hosted assets before sending.
4. Update CTA `href` values and UTM parameters to match your campaign.
