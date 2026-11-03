# Kora Store: Responsive Store Landing Page

A responsive landing page for an online clothing store, built with HTML, CSS and Bootstrap 5.

## Files

- `index.html`: the page structure (header, hero, product section, extra sections, footer)
- `styles.css`: all custom styling and the media queries
- `images/`: four product illustrations (SVG, so they stay sharp on any screen)
- `screenshots/`: the page on desktop, tablet and mobile, plus the mobile menu opened

## How to run

Keep the files in the same folder and open `index.html` in a browser. An internet connection is needed to load Bootstrap and the Roboto font.

## Design choices

**Colour.** A deep navy with a single amber accent. Navy gives the page a trustworthy, clean feel, and amber is used only for things the visitor should act on: the main buttons, the announcement of the sale, and the logo highlight. Light grey sections separate the content without heavy borders.

**Typography.** Roboto throughout, as the brief required. Weight does the work of hierarchy: heavy for the hero headline, bold for section titles and prices, light for supporting text.

**Layout.** The page follows the order a shopper expects: a hero that says what the store offers, the best sellers, reasons to trust the store, an offer to sign up, then the footer. Content sits in a centred container so lines never get too long on wide screens.

**Product cards.** Each card has the same structure: image, name, short description, price and a Shop Now button. The price and button are pinned to the bottom of the card, so all four buttons line up even when descriptions have different lengths. Cards lift slightly on hover to show they are interactive. Small badges (New, Sale) draw attention to certain items.

**Images.** The product pictures are simple SVG illustrations, so the project has no copyright problems and loads fast. Replace them with real photos by changing the `src` of each image.

## Responsive design

The layout is built mobile friendly in two ways.

1. **Bootstrap grid.** The product cards use `col-12 col-sm-6 col-lg-3`, which gives one card per row on phones, two on tablets and four on desktop. The navbar collapses into a menu button on screens narrower than 992px.
2. **Custom media queries in `styles.css`.** There are three breakpoints:
   - Under 992px (tablets): smaller hero headline, hero text centred above a smaller image, less section spacing, and tidy borders between menu links.
   - Under 768px (large phones): smaller section titles and a centred footer.
   - Under 576px (small phones): the smallest headline, full width hero buttons that are easy to tap, and the tightest spacing.

The page was checked at 1440px (desktop), 820px (tablet) and 390px (phone) wide, with no sideways scrolling at any size.

## Bootstrap features used (extra points)

- Grid system (`container`, `row`, `col-*`, gap utilities)
- Responsive navbar with the collapse menu button
- Cards for the products
- Buttons and badges
- Input group for the newsletter form
- Utility classes for spacing, flexbox and alignment

## Code notes

Both files use comments to mark each section, and class names describe what each element is (`product-card`, `hero-title`, `footer-link`).
