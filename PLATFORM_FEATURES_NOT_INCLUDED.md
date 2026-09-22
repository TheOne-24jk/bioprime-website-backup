# Platform-only features not included

- **Server runtime:** the original build can run through a Cloudflare-compatible
  worker. The static export instead contains the already rendered homepage and
  browser bundles.
- **Runtime middleware:** response headers formerly emitted by middleware were
  translated into `_headers`; the host must support that file for HTTP-level
  enforcement.
- **Sites hosting controls:** deployments, version history, custom-domain
  configuration, publication status, and workspace access controls remain in
  ChatGPT Sites.
- **Dynamic React Server Component navigation:** the live worker can generate
  fresh RSC responses. The export is a single static route and does not include
  that server endpoint.

The current Site declares no D1 database and no R2 object-storage binding. No
application authentication, API routes, uploads, server-side forms, secrets,
environment files, or customer databases were found in the exported source.
