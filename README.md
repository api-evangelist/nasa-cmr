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

This repository contains an APIs.json 0.19 profile for the NASA CMR API suite maintained by [api-evangelist](https://github.com/api-evangelist).

## APIs

| API | Base URL | Description |
|-----|----------|-------------|
| CMR Search | `https://cmr.earthdata.nasa.gov/search` | RESTful search across collections, granules, variables, services, and tools |
| CMR Ingest | `https://cmr.earthdata.nasa.gov/ingest` | Create and update metadata records (provider auth required) |
| CMR Access Control | `https://cmr.earthdata.nasa.gov/access-control` | Manage ACLs and check user permissions |
| CMR GraphQL | `https://graphql.earthdata.nasa.gov/api` | Unified GraphQL interface to all CMR resources |
| CMR STAC | `https://cmr.earthdata.nasa.gov/stac` | STAC-compliant catalog organized by provider |
| CMR OpenSearch | `https://cmr.earthdata.nasa.gov/opensearch` | OpenSearch-compliant discovery interface |

## Authentication

- **Public search**: No authentication required for publicly available metadata
- **Restricted collections**: EDL Bearer Token (`Authorization: Bearer <token>`) from [Earthdata Login](https://urs.earthdata.nasa.gov/)
- **Metadata ingest**: EDL Bearer Token (Level 4 MFA) or Launchpad SAML Token (Level 5), plus provider ACL authorization

## Rate Limits

CMR does not publish fixed numeric rate limits. Throttling rules are applied per request signature. HTTP 429 responses include a `retry-after` header that clients must honor. Key constraints:

- Request timeout: 180 seconds (170s internal, returns partial results)
- Max page size: 2,000 results (default: 10)
- Max GET URL length: 6,000 characters (use POST for complex queries)
- Deep paging limit: 1 million items via `CMR-Search-After` header

## Pricing

All CMR APIs are free public services. No subscription fees, per-request charges, or registration costs apply. Data file access (granule downloads) may incur egress charges at the DAAC level.

## Resources

- [CMR Search API Docs](https://cmr.earthdata.nasa.gov/search/site/docs/search/api.html)
- [CMR Ingest API Docs](https://cmr.earthdata.nasa.gov/ingest/site/docs/ingest/api.html)
- [CMR Access Control API Docs](https://cmr.earthdata.nasa.gov/access-control/site/docs/access-control/api.html)
- [CMR GraphQL Docs](https://graphql.earthdata.nasa.gov/docs/introduction/introduction/)
- [CMR STAC GitHub](https://github.com/nasa/cmr-stac)
- [CMR Source Code](https://github.com/nasa/Common-Metadata-Repository)
- [Earthdata Login](https://urs.earthdata.nasa.gov/)
- [Earthdata Forum](https://forum.earthdata.nasa.gov/)
- [Status Page](https://status.earthdata.nasa.gov/)
