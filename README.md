# swellstack.github.io

Public-facing home page + privacy policy for SwellStack — plain static HTML (no build step, no
Jekyll — see `.nojekyll`), served as-is by GitHub Pages.

This exists specifically to satisfy Google's OAuth branding verification for
**Authentication-api**'s "Sign in with Google" (see `GoogleAuth:ClientId` in that repo): Google
requires a public, unauthenticated home page that explains the app's purpose and links to a
substantive privacy policy. It is not a marketing site for a consumer product — SwellStack's
tools (MyVault, LineEdge, etc.) are internal.

## Structure

- `index.html` — home page.
- `privacy/index.html` — privacy policy, linked from the home page (served at `/privacy`).

## Editing

Plain HTML/CSS, no dependencies. Edit the files directly and push to `main` — GitHub Pages
publishes on every push.

## Google Search Console verification

`index.html` has a commented-out spot for the `google-site-verification` meta tag. Get the code
from [Search Console](https://search.google.com/search-console) → Add property → `https://swellstack.github.io` →
HTML tag method → paste the code in, uncomment, push.
