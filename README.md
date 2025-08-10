# Shopify Tailwind Starter (Minimal)

A minimal Shopify theme scaffold styled with Tailwind CSS—no bundlers, no unnecessary packages.

## Features
- Online Store 2.0 JSON templates for essential pages
- Tailwind CSS via CLI only
- Minimal sections/snippets to get started fast
- Clean, semantic markup with accessible defaults

## Getting Started

1. Install dependencies:
   ```
   npm install
   ```

2. Build CSS:
   - Dev (watch):
     ```
     npm run dev:css
     ```
   - Production build:
     ```
     npm run build:css
     ```

   This generates `assets/theme.css`.

3. Serve with Shopify CLI:
   ```
   npx @shopify/cli theme dev
   ```
   Or if you have it installed:
   ```
   shopify theme dev
   ```

4. Deploy:
   ```
   shopify theme push
   ```

## Structure
- `layout/` — theme layout (header/footer sections are included here)
- `templates/` — JSON templates for OS 2.0 pages
- `sections/` — reusable page sections
- `snippets/` — smaller reusable UI parts
- `assets/` — compiled CSS (`theme.css`)
- `src/styles/input.css` — Tailwind entry for CSS

## Notes
- Header/footer live in `layout/theme.liquid` via `{% section %}` for consistency.
- Keep things minimal. Add only what you need.