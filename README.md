# Hayroo — Premium E-commerce

Hayroo is a full-stack e-commerce application built with a React client and a Node.js/Express server.

## Current repository status

The repository currently contains the project overview, security checklist, safe environment templates, and the premium UI implementation roadmap. The original application source from the uploaded ZIP has **not yet been transferred into this repository**.

## Planned application structure

- `client/` — React storefront and admin dashboard
- `server/` — Express API, authentication, product/order/category controllers, and database configuration
- `docs/` — implementation and security notes

## Design direction

The upgrade target is a premium Apple-inspired experience: restrained typography, generous spacing, refined surfaces, subtle depth, and buttery-smooth interactions across the storefront, cart, product pages, customer account, and admin dashboard.

## Setup

When the application source is added:

1. Install a supported Node.js LTS version.
2. Install dependencies in `client/` and `server/`.
3. Copy `client/.env.example` to `client/.env` and `server/.env.example` to `server/.env`.
4. Fill in local configuration values; never commit real secrets.
5. Use Braintree sandbox credentials until checkout testing is complete.

See [the implementation roadmap](docs/implementation-roadmap.md) and [security notes](SECURITY.md).

## Security

Environment files, logs, dependency directories, build outputs, and generated uploads should not be committed. Rotate any payment credential that may have been exposed. Review server-side authorization and deployment settings before going live.
