# NASA CMR

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

NASA Common Metadata Repository (CMR) is a high-performance metadata system that catalogs Earth science data collections, granules, variables, services, and tools across NASA data centers. It provides REST, GraphQL, STAC, OpenSearch, and CSW interfaces for discovering, searching, and ingesting metadata for satellite and Earth observation datasets spanning decades of NASA missions.

**Areas:** NASA · Earth Science · Satellite Data · Remote Sensing · Geospatial · Open Data · Metadata · Collection · Granules

## NASA CMR on APIs.io

Everything profiled for NASA CMR is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/nasa-cmr/](https://apis.io/providers/nasa-cmr/)** — or go straight to one of the APIs or properties below.

### APIs (9)

- [CMR Ingest API](https://apis.io/apis/nasa-cmr/cmr-ingest/) — REST API for creating, updating, and deleting metadata records in the Common Metadata Repository. Supports collections, granules, variables, services,…
- [CMR Access Control API](https://apis.io/apis/nasa-cmr/cmr-access-control/) — REST API for managing Access Control Lists (ACLs) and checking user permissions across CMR concepts. Supports system, provider, single-instance, and…
- [CMR GraphQL API](https://apis.io/apis/nasa-cmr/cmr-graphql/) — Unified GraphQL interface for querying the Common Metadata Repository. Provides a single endpoint to search collections, granules, variables, tools,…
- [CMR STAC API](https://apis.io/apis/nasa-cmr/cmr-stac/) — SpatioTemporal Asset Catalog (STAC) compliant API wrapping the CMR Search API. Organizes the full NASA CMR catalog by provider and enables discovery of STAC…
- [CMR OpenSearch API](https://apis.io/apis/nasa-cmr/cmr-opensearch/) — OpenSearch-compliant API wrapper for CMR Search enabling standard OpenSearch client integration. Supports collection discovery with spatial and temporal…
- [NASA CMR Capabilities API](https://apis.io/apis/nasa-cmr/nasa-cmr-capabilities-api/) — essential characteristics of this API
- [NASA CMR Collections API](https://apis.io/apis/nasa-cmr/nasa-cmr-collections-api/) — Collection Search
- [NASA CMR Data API](https://apis.io/apis/nasa-cmr/nasa-cmr-data-api/) — access to data (features)
- [NASA CMR STAC API](https://apis.io/apis/nasa-cmr/nasa-cmr-stac-api/) — Extension to WFS3 Core to support STAC metadata model and search API

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### GraphQL (1)

GraphQL schemas.

- [NASA CMR GraphQL API](https://apis.io/graphqls/nasa-cmr/nasa-cmr-graphql/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Nasa Cmr Agentic Access](https://apis.io/agentic-access/nasa-cmr/nasa-cmr-agentic-access/)

#### JSON Schema (6)

The data models the API reads and writes.

- [NASA CMR STAC Collection](https://apis.io/schemas/nasa-cmr/nasa-cmr-stac-collection/)
- [NASA CMR STAC Featurecollectiongeojson](https://apis.io/schemas/nasa-cmr/nasa-cmr-stac-featureCollectionGeoJSON/)
- [NASA CMR STAC Featuregeojson](https://apis.io/schemas/nasa-cmr/nasa-cmr-stac-featureGeoJSON/)
- [NASA CMR STAC Landingpage](https://apis.io/schemas/nasa-cmr/nasa-cmr-stac-landingPage/)
- [Link](https://apis.io/schemas/nasa-cmr/nasa-cmr-stac-link/)
- [NASA CMR STAC Searchbody](https://apis.io/schemas/nasa-cmr/nasa-cmr-stac-searchBody/)

#### JSON-LD (2)

Linked-data contexts for the provider's vocabulary.

- [Nasa Cmr Context](https://apis.io/jsonld/nasa-cmr/nasa-cmr-context/)
- [Nasa Cmr Dataset Context](https://apis.io/jsonld/nasa-cmr/nasa-cmr-dataset/)

#### Examples (4)

Example requests and responses.

- [Nasa Cmr Ingest Collection Request](https://apis.io/examples/nasa-cmr/nasa-cmr-ingest-collection-request/)
- [Nasa Cmr Search Collections Response](https://apis.io/examples/nasa-cmr/nasa-cmr-search-collections-response/)
- [Nasa Cmr Search Granules Response](https://apis.io/examples/nasa-cmr/nasa-cmr-search-granules-response/)
- [Nasa Cmr Stac Landing Page](https://apis.io/examples/nasa-cmr/nasa-cmr-stac-landing-page/)

#### Collections (4)

Postman and Open Collection request collections.

- [CMR Search Capabilities API](https://apis.io/collections/nasa-cmr/open-nasa-cmr-capabilities-api/)
- [CMR Search Capabilities Collections API](https://apis.io/collections/nasa-cmr/open-nasa-cmr-collections-api/)
- [CMR Search Capabilities Data API](https://apis.io/collections/nasa-cmr/open-nasa-cmr-data-api/)
- [CMR Search Capabilities STAC API](https://apis.io/collections/nasa-cmr/open-nasa-cmr-stac-api/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [NASA CMR — jsonschema rules](https://apis.io/rules/nasa-cmr/nasa-cmr-jsonschema-spectral-rules/)

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Nasa Cmr Domain Security](https://apis.io/security/nasa-cmr/nasa-cmr-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Nasa Cmr Plans Pricing](https://apis.io/plans/nasa-cmr/nasa-cmr-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Nasa Cmr Rate Limits](https://apis.io/rate-limits/nasa-cmr/nasa-cmr-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Nasa Cmr Finops](https://apis.io/finops/nasa-cmr/nasa-cmr-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.earthdata.nasa.gov/about/esdis/eosdis/cmr)
- [Documentation](https://www.earthdata.nasa.gov/engage/open-data-services-software/earthdata-developer-portal/cmr-api)
- [Blog](https://www.earthdata.nasa.gov/news)
- [Status](https://status.earthdata.nasa.gov/)

## API Evangelist rating

**Kin Score 33.4** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 55.7 |
| Contract governance | 9.8 |
| Operational transparency | 44.7 |
| Developer ergonomics | 16.7 |
| Access clarity | 14.5 |

**Agent readiness 15.4** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | — |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 10.8** — Government & Public Sector

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/nasa-cmr/](https://apis.io/providers/nasa-cmr/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for NASA CMR: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/nasa-cmr/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
