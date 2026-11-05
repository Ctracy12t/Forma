# Forma deployment

The static site lives in `dist/index.html`. `vercel.json` sets the output directory and HTTP security headers. The existing Vercel project is `forma-listing-films` in the `forma-ba97` workspace.

- Site: https://forma-listing-films.vercel.app
- Source snapshot: `9413cbeef149f719f743db0c3ad5abb30c514334`
- Deployment method at time of backup: direct source upload to Vercel

To preview locally, run `python3 -m http.server --directory dist 8000` from the repository root and open `http://localhost:8000`. No build step or application environment variables are required for this static page. Update the CSP hash in `vercel.json` if the inline stylesheet changes.

Checkout uses Stripe test mode. Order intake, payment verification, video production, and delivery are future work. Vercel workspace permissions and deployment protection are managed in Vercel.
