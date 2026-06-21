# Hymadeck Solar Solution

Hymadeck Solar Solution manages the full journey from equipment sourcing to installation and ongoing maintenance for residential, commercial, and industrial solar projects. This project is a polished static website concept designed to showcase their brand, services, and portfolio.

## Folder Structure

The project has been organized for better maintainability:

```text
/
├── index.html          # Homepage
├── pages/              # Additional pages
│   ├── about.html      # About page
│   ├── contact.html    # Contact page
│   ├── projects.html   # Projects portfolio
│   └── services.html   # Services offered
├── css/
│   └── style.css       # Global styles (custom CSS properties, typography, layout)
├── js/
│   └── main.js         # Global interactive logic (e.g., Theme toggling)
├── assets/             # Images and SVG icons (e.g., logo.svg, favicon.svg)
└── README.md           # Project documentation
```

## Setup & Local Development

This is a static website consisting of plain HTML, CSS, and JS.

To view the website locally:
1. Clone or download this repository.
2. Open `index.html` in your favorite web browser.
3. For a better development experience (e.g., to resolve relative paths or test module loading if added later), run a local development server:
   - Using Python: `python3 -m http.server 8000`
   - Using Node.js: `npx serve` or `npx live-server`
4. Navigate to `http://localhost:8000` (or whichever port your server uses) in your browser.

## Technologies Used

- **HTML5:** Semantic HTML markup.
- **CSS3:** Modern CSS including Flexbox, CSS Grid, Custom Properties (variables), and a responsive design approach without the need for an external CSS framework.
- **Vanilla JavaScript:** For interactive elements such as dark/light mode toggling based on system preferences.
- **Fonts:** Custom typography using `General Sans` and `Cabinet Grotesk` from Fontshare.

## Customization and Styling

The styling relies heavily on CSS variables (Custom Properties) defined at the top of `css/style.css`.
You can easily customize the site's theme by modifying these variables:

- `--color-primary`, `--color-bg`, `--color-text`, etc.
- Font scales and spacing tokens (`--text-*` and `--space-*`)

The site includes a built-in dark mode which can be toggled using the button in the navigation header, or it will fall back to your OS's preferred color scheme.

## Premium Upgrade & E-commerce Strategy

The site has been upgraded to a premium business layout featuring refined colors, enhanced typography, and trust signals (warranties, certifications, partner logos).

### E-commerce Implementation Note
To add e-commerce without abandoning the fast, secure, and maintainable static HTML architecture, we have integrated **Snipcart**. Snipcart provides a drop-in shopping cart and checkout modal that injects directly into the static site.

- **Shop Page (`pages/shop.html`):** Displays the product catalog.
- **Product Detail (`pages/product.html`):** Displays deep-dives into specific products.
- **Cart & Checkout (`pages/cart.html` & `pages/checkout.html`):** These pages redirect to the Shop page. This is because Snipcart natively handles cart and checkout globally via a UI overlay triggered by the "Cart" buttons in the navigation header, meaning dedicated HTML pages for these flows are unnecessary and redundant in this stack.

### Follow-up Work for Live E-commerce
Before accepting real payments, the following steps must be completed:
1. **Snipcart Account:** Create an account at [snipcart.com](https://snipcart.com) and replace the placeholder `data-api-key` in `js/main.js` or the global HTML with your Live API key.
2. **Domain Verification:** Snipcart requires the site to be hosted on a public domain to verify product prices securely.
3. **Payment Gateway:** Connect a payment gateway (e.g., Paystack, Flutterwave, or Stripe depending on your region) inside the Snipcart dashboard.
4. **Shipping & Taxes:** Configure shipping rates (e.g., flat rate or weight-based via custom fields) and applicable taxes in the Snipcart dashboard.
5. **Real Product Data:** Update the `data-item-*` attributes on the "Add to Cart" buttons in `shop.html` and `product.html` with your actual product IDs, prices, names, and image URLs.
