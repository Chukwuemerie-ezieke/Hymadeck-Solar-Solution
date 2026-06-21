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
