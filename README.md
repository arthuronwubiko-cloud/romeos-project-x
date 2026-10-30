# Romeo's Pizza Project

A small, static website for Romeo's Pizza. It has a home page and a separate
full-menu page, built with plain HTML and CSS. There is no framework, build
step, server-side code, or JavaScript application.

## Project files

All site files are in [`peter hustle/`](./peter%20hustle/).

| File | Purpose |
| --- | --- |
| [`peter890.html`](./peter%20hustle/peter890.html) | Home page structure and content. |
| [`peter890.css`](./peter%20hustle/peter890.css) | Home page layout, colors, typography, interactions, and responsive styles. |
| [`890b.html`](./peter%20hustle/890b.html) | Full menu page structure and content. |
| [`890b.css`](./peter%20hustle/890b.css) | Full menu page layout, pizza cards, buttons, and responsive styles. |

Keep each HTML file beside its matching CSS file: the pages load their styles
using relative paths (`peter890.css` and `890b.css`).

## Pages and content

### Home page — `peter890.html`

The home page is arranged from top to bottom:

1. **Header:** Romeo's logo, links to the home page, menu, and locations, plus
   an order link and a search-field design.
2. **Hero:** A short introduction, order button, and featured pizza image.
3. **Menu preview:** Three cards for pizza, shawarma, and chicken wings. The
   “View full menu” link opens `890b.html`.
4. **Locations:** Store cards grouped under Abuja and Lagos.
5. **Pizza gallery:** A horizontally scrollable strip of pizza photos.
6. **Footer:** The logo, motto, and social-sharing links.

### Full menu — `890b.html`

The full menu is arranged as:

1. **Header:** The logo and links to the home page, pizza menu, and pizza deals.
2. **Menu introduction:** A breadcrumb, description, hero photo, and button
   that jumps to the traditional pizza section.
3. **Pizza categories:** Traditional, special, and exclusive pizzas, each shown
   as cards with an image, description, price, and order button.
4. **Sides:** Chicken wings and shawarma roll cards.
5. **Pizza deals:** A placeholder section with a link back to the menu.
6. **Footer:** Navigation back to the home page and to menu sections.

## How the code works

HTML provides the content and structure. Elements such as `<header>`, `<nav>`,
`<main>`, `<section>`, `<article>`, and `<footer>` identify the role of each
part of the page. Classes (for example, `pizza-card` and `menu-hero`) connect
HTML elements to their CSS rules.

CSS controls appearance and layout. The home hero and menu hero use CSS Grid;
navigation bars, card contents, and footers use Flexbox. CSS Grid also lays out
the menu and location cards. Shared visual rules style typography, colors,
spacing, buttons, and image crops. Hover and keyboard-focus selectors provide
interaction feedback.

Both stylesheets use media queries to adapt the layout to smaller screens. The
home page changes its hero and card grids at tablet and phone widths. The menu
page changes from three pizza columns to two at tablet width, then to one at
phone width; its hero also stacks its text and image vertically on phones.

Internal links use URL fragments. For example, `href="#traditional"` scrolls
to the element whose `id` is `traditional`. Keep the target `id` and link
fragment in sync when renaming or moving sections.

## Run locally

Open `peter hustle/peter890.html` directly in a modern browser. Choose **Menu**
or **View full menu** to open `890b.html`; use the menu page's **Home** link to
return. No package installation or compilation is required.

Most images are loaded from Romeo's Pizza's website or Unsplash, and the home
page loads Font Awesome from a CDN. Those external assets require an internet
connection. If an external image URL changes or becomes unavailable, replace
its `src` value with another public image URL.

## Editing guide

- To change page text, prices, or menu items, edit the corresponding HTML.
- To add a menu item, copy an existing `<article class="pizza-card">` in the
  appropriate category and update its image, alternative text, name,
  description, and price.
- To add a section link, give the destination an `id` and link to it with
  `href="#that-id"`.
- To change styling, edit the matching stylesheet. Use the existing class
  names and media-query breakpoints to keep desktop and mobile layouts
  consistent.
- Give each meaningful image descriptive `alt` text. Decorative images can use
  an empty `alt=""` so assistive technology skips them.

## Current limitations

- The home page's search field is only a visual input; no search behavior is
  implemented.
- The full-menu **ORDER NOW** buttons use `href="#"` placeholders and do not
  place orders. The home-page order links currently open Romeo's Facebook page.
- The pizza-deals section is placeholder content.
- There is no JavaScript, back-end, or ordering integration.
