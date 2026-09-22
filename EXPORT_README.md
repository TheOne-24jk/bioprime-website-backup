# BioPrime portable static export

Source: latest synchronized version of https://bioprimecollagen.com  
Site version: 8  
Source commit: `ebb9b2a195a4a3fea3e29ef436f52588cf5e4192`

## Deploy

Upload the contents of this folder to any static web host, keeping `index.html`
at the web root and preserving all paths. The `_headers` file carries the
security and caching policy for hosts that support that convention.

For a local check, serve this directory over HTTP rather than opening
`index.html` directly, because browsers restrict JavaScript modules loaded by
the `file:` protocol.

## Included

- Fully rendered root `index.html`
- Minified, content-hashed CSS and JavaScript bundles
- Responsive product imagery in PNG and WebP formats
- Logo and favicon SVG assets
- Search metadata (`robots.txt`, `sitemap.xml`, canonical and social metadata)
- Security policy in both the HTML CSP meta tag and `_headers`
- Long-lived caching for hashed build assets and bounded image caching

## Not part of the static export

- ChatGPT Sites deployment/runtime and custom-domain management
- The platform's server worker, request middleware, and dynamic RSC responses
- Platform access-control enforcement

No database, object storage, user authentication, form backend, API route, or
server-side customer-data store is used by this Site. Ordering and questions
continue through the external Messenger link and therefore require internet
access and Facebook Messenger availability.
