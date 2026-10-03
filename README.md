# Copy-ready Cinder docs

This directory contains **37 MDX content pages**, with Mintlify-compatible
frontmatter and native field/example components. Copy the pages and folder structure
into your existing Mintlify documentation repository. Add their extensionless
paths to that repository's navigation configuration. No new site, package,
application, hosting account or deployment configuration is included here.

Suggested navigation:

- Start: `index`, `status`, `quickstart`.
- Guides: `guides/accounts`, `guides/funds`, `guides/trading`, `guides/agents`.
- Security: `security/privacy`, `security/risk`, `security/recovery`,
  `security/verification`.
- API: `api/overview`, `api/authentication`, `api/units`, `api/lifecycle`,
  `api/errors`.
- Commands: all eight pages under `api/methods/`.
- Reads: `api/reads/paging` and all ten family pages under `api/reads/`.
- Socket: `api/websocket`, `api/limits`.

Links use Mintlify root-relative, extensionless page routes. If you nest the
content under a prefix in your docs repository, adjust those links accordingly.
Command/read pages use `api: "POST /v1/exchange"` for the real shared carrier and
`playground: "none"`: the request fields describe SDK objects, not a directly
callable JSON body. `RequestExample` and `ResponseExample` show examples alongside
the `ParamField`/`ResponseField` schemas; `Expandable` groups nested fields.
Your existing Mintlify theme/navigation remain yours. No base URL is invented.
This README is a copying note, not a public navigation page. Example methods use
the configured client/context described in the quickstart; there is no live
endpoint, self-service account API or published npm SDK implied.

Content is based on merged P21A implementation `0530374` and the approved
financial/privacy/recovery baseline. Commands, units, permissions, uncertainties
and limits are mapped to the tracked TypeScript/Rust sources. Validation receipts
live in the implementation tracker; they do not imply hosted publication, a live
endpoint or customer-funds qualification. There is no conversion to MD, new
recurring CI requirement or runtime change.
