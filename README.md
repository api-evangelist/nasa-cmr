# NASA CMR

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
