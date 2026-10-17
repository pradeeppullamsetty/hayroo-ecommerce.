# Security Notes

Before deployment:

- Never commit `.env` files or real credentials.
- Use separate development and production secrets.
- Rotate any Braintree private key or other secret that may have been exposed.
- Keep payment processing in sandbox mode until end-to-end tests pass.
- Restrict CORS to the deployed frontend origin.
- Ensure admin endpoints enforce server-side authorization; hiding UI controls is not authorization.
- Validate and sanitize user input on the server.
- Apply upload size/type limits and do not serve private uploads publicly.
- Use HTTPS in production and configure secure cookies/session settings where applicable.
- Do not store card details in the application database.
- Review dependency vulnerabilities before release.

This document is a checklist, not a claim that every item has already been verified.
