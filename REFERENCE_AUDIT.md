# Reference audit

Result: **pass**

- Every local stylesheet, script, image, and SVG referenced by `index.html`
  exists in the export.
- Local HTML references use portable relative paths (`./_next/...` and
  `./images/...`).
- No local computer paths were found.
- No missing local references were found.
- No environment files, API keys, access tokens, private keys, bearer tokens,
  or embedded credentials were found.

Intentional absolute web references:

- `https://bioprimecollagen.com` — canonical and social-sharing metadata
- `https://m.me/586756427844484` — external Messenger ordering/support flow
- `https://doi.org/10.3390/nu10070826` — research citation
- `https://doi.org/10.1111/jocd.12174` — research citation

Fragment-only links (`#ingredient`, `#ritual`, `#questions`, and `#quiz`) target
elements present in `index.html`.
