# Hayroo premium UI upgrade plan

## Direction
Apple-inspired minimal premium design with restrained violet accents, spacious layouts, clean typography, fine borders, soft depth, and buttery-smooth interactions. The current React/Express/MongoDB/Braintree architecture is retained during the visual pass.

## Included in this preparation pass
- Added `client/src/hayroo-design-system.css` as a global progressive enhancement layer.
- Imported the design layer from the React entry point.
- Added reduced-motion support and visible keyboard focus styles.
- Added `.env.example` templates for client and server.
- Removed real `.env` files from the prepared source tree and expanded `.gitignore` to exclude secrets and generated output.

## Next implementation stages
1. Run frontend/backend installs and establish baseline build/runtime status.
2. Refactor shared storefront header/footer and responsive navigation.
3. Refresh home hero, category browsing, product cards, search/filter, and product details.
4. Polish cart, wishlist, authentication, checkout and order history; preserve API contracts.
5. Refresh admin sidebar, overview cards, product/category forms, orders tables, loading/error/empty states.
6. Verify authentication/authorization, API integration, payment sandbox flow, accessibility, mobile layouts and performance.
7. Add deployment setup and publish only after reviewing secrets and build status.

## Security notes
- Do not commit `.env` files or live credentials.
- Rotate any Braintree private key that has been exposed outside the private development environment.
- Use sandbox credentials for testing; verify webhook and server-side transaction validation before production.
- `client/.env.example` and `server/.env.example` are templates only and must be filled with deployment-specific values.

## Current limitations
The global layer is intentionally progressive and does not yet replace the bespoke layout of every page. Page-level redesign and integration tests are the next phase, not claimed as completed by this preparation pass.
