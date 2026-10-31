# Romeo's Pizza Project

A static restaurant website for Romeo's Pizza Nigeria. The project includes a home page, a full menu page, and a deals page, all built with plain HTML and CSS with no framework, build step, or backend.

## Project structure

```text
.
├── index.html
├── 890b.html
├── pizzadeals.html
├── peter890.css
├── README.md
├── .gitattributes
└── .DS_Store
```

## Files

| File | Purpose |
| --- | --- |
| [`index.html`](./index.html) | Home page with hero section, menu highlights, locations, gallery, and footer. |
| [`890b.html`](./890b.html) | Full menu page with pizza categories, sides, and menu CTA sections. |
| [`pizzadeals.html`](./pizzadeals.html) | Deals page with featured offers, combo packages, and promo content. |
| [`peter890.css`](./peter890.css) | Shared styling for all pages: layout, colors, typography, buttons, responsiveness, and hover states. |
| [`README.md`](./README.md) | Project overview, usage notes, and editing guide. |

## Pages and content

### Home page — `index.html`

The home page includes:

1. Header navigation with Home, Menu, Locations, Deals, and Order links.
2. Hero section with a featured pizza image and call-to-action button.
3. Menu preview cards for pizza, shawarma, and chicken wings.
4. Locations section grouped by Abuja and Lagos stores.
5. Horizontally scrollable pizza gallery.
6. Footer with branding and social-share links.

### Full menu — `890b.html`

The menu page includes:

1. Header and navigation to the home page and deals.
2. Menu hero with breadcrumb, description, and jump link to pizza categories.
3. Traditional, special, and exclusive pizza sections.
4. Sides and add-on items.
5. Pizza deals placeholder section.
6. Footer navigation.

### Deals page — `pizzadeals.html`

The deals page includes:

1. Hero banner for the pizza offers.
2. Intro text for special value deals.
3. Deal cards showing combo pricing and product details.
4. Promotional image panels and CTA buttons.
5. Footer with branding and social links.

## How the code works

- HTML provides the content and page structure.
- CSS handles layout, colors, spacing, typography, buttons, hover effects, and responsive behavior.
- The same stylesheet (`peter890.css`) is linked by all pages.
- The site uses CSS Grid and Flexbox for alignment and page layout.
- Media queries adjust layout for tablet and mobile screens.
- Internal links use section IDs and page navigation links for smooth movement between pages.

## Run locally

You can open any HTML file directly in a browser, or serve the project locally with a simple web server.

Example:

```bash
python -m http.server 8000
```

Then open:

- `http://localhost:8000/index.html`
- `http://localhost:8000/890b.html`
- `http://localhost:8000/pizzadeals.html`

No package installation or build step is required.

## Notes

- Most images are loaded from Romeo's Pizza or Unsplash.
- Font Awesome is loaded from a CDN for icons.
- If an external image or font URL changes or fails, replace the `src` or stylesheet link with a valid alternative.

## Editing guide

- Update page content, pricing, and menu items in the relevant HTML file.
- Update shared styling in `peter890.css`.
- Keep class names consistent when editing CSS to preserve the site layout.
- Add descriptive `alt` text for meaningful images.
- Use section IDs and matching anchor links when adding new in-page navigation.

## Current limitations

- The search field on the home page is presentational only and does not filter content.
- Some order buttons still point to placeholder or external links rather than a real checkout flow.
- The menu page contains placeholder deal content.
- There is no JavaScript-driven shopping cart, ordering form, or backend integration.
- The website is static and intended for promotional/display purposes.

## License

This project does not currently include a license file. If you plan to publish or share it publicly, add an appropriate license before distribution.
