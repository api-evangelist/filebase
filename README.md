# Filebase

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

Filebase is an S3-compatible object storage and IPFS pinning platform that combines familiar cloud storage APIs with decentralized, blockchain-backed infrastructure. Developers can store, manage, and pin files to IPFS using standard S3 tooling, a dedicated IPFS Pinning Service API, and an IPFS RPC API — all without changing existing workflows. Filebase delivers geo-redundant 3x replication, free egress for object storage, a global CDN, and predictable pricing, making it straightforward to build Web3 applications on top of decentralized networks through a Web2-style developer experience.

**Areas:** Object Storage · IPFS · S3 Compatible · Decentralized Storage · Pinning · Web3 · Cloud Storage · Blockchain · Storage

## Filebase on APIs.io

Everything profiled for Filebase is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/filebase/](https://apis.io/providers/filebase/)** — or go straight to one of the APIs or properties below.

### APIs (15)

- [Filebase S3-Compatible API](https://apis.io/apis/filebase/filebase-s3-api/) — The Filebase S3-Compatible API provides standard AWS S3 protocol support for bucket and object management. Developers can use any existing S3 SDK, CLI tool,…
- [Filebase Platform API](https://apis.io/apis/filebase/filebase-platform-api/) — The Filebase Platform API provides account-level operations that complement the S3 API. Using HTTP Basic authentication with base64-encoded access key and…
- [Filebase IPFS Pinning Service API](https://apis.io/apis/filebase/filebase-ipfs-pinning-service-api/) — The Filebase IPFS Pinning Service API implements the vendor-neutral IPFS Pinning Service specification. Per-bucket Bearer tokens authenticate requests to…
- [Filebase IPFS RPC API](https://apis.io/apis/filebase/filebase-ipfs-rpc-api/) — The Filebase IPFS RPC API exposes core IPFS daemon functionality through an HTTP interface. Bucket-specific Bearer tokens authenticate all POST requests to…
- [Filebase Buckets API](https://apis.io/apis/filebase/filebase-buckets-api/) — Per-bucket storage consumption
- [Filebase Data Management API](https://apis.io/apis/filebase/filebase-data-management-api/) — Add, retrieve, and import IPFS data
- [Filebase IPNS API](https://apis.io/apis/filebase/filebase-ipns-api/) — IPNS name publishing and resolution
- [Filebase Keypairs API](https://apis.io/apis/filebase/filebase-keypairs-api/) — IPNS keypair management
- [Filebase MFS API](https://apis.io/apis/filebase/filebase-mfs-api/) — Mutable File System operations
- [Filebase Multipart Upload API](https://apis.io/apis/filebase/filebase-multipart-upload-api/) — Large file multipart upload operations
- [Filebase Node API](https://apis.io/apis/filebase/filebase-node-api/) — IPFS node information
- [Filebase Objects API](https://apis.io/apis/filebase/filebase-objects-api/) — Object upload, download, copy, delete, and metadata
- [Filebase Pinning API](https://apis.io/apis/filebase/filebase-pinning-api/) — Pin and unpin IPFS objects
- [Filebase Pins API](https://apis.io/apis/filebase/filebase-pins-api/) — IPFS pin management operations
- [Filebase Usage API](https://apis.io/apis/filebase/filebase-usage-api/) — Account-level usage and bandwidth metrics

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Filebase Agentic Access](https://apis.io/agentic-access/filebase/filebase-agentic-access/)

#### JSON Schema (3)

The data models the API reads and writes.

- [Filebase Pin](https://apis.io/schemas/filebase/filebase-pin/)
- [Filebase Pin Status](https://apis.io/schemas/filebase/filebase-pin-status/)
- [Filebase Usage Metrics](https://apis.io/schemas/filebase/filebase-usage/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Filebase Context](https://apis.io/jsonld/filebase/filebase-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Filebase Vocabulary](https://apis.io/vocabularies/filebase/filebase-vocabulary/)

#### Examples (4)

Example requests and responses.

- [Filebase Add Ipfs Response Example](https://apis.io/examples/filebase/filebase-add-ipfs-response-example/)
- [Filebase Pin Example](https://apis.io/examples/filebase/filebase-pin-example/)
- [Filebase Pin Status Example](https://apis.io/examples/filebase/filebase-pin-status-example/)
- [Filebase Usage Example](https://apis.io/examples/filebase/filebase-usage-example/)

#### Collections (11)

Postman and Open Collection request collections.

- [Filebase IPFS Pinning Service Buckets API](https://apis.io/collections/filebase/open-filebase-buckets-api/)
- [Filebase IPFS Pinning Service Buckets Data Management API](https://apis.io/collections/filebase/open-filebase-data-management-api/)
- [Filebase IPFS Pinning Service Buckets IPNS API](https://apis.io/collections/filebase/open-filebase-ipns-api/)
- [Filebase IPFS Pinning Service Buckets Keypairs API](https://apis.io/collections/filebase/open-filebase-keypairs-api/)
- [Filebase IPFS Pinning Service Buckets MFS API](https://apis.io/collections/filebase/open-filebase-mfs-api/)
- [Filebase IPFS Pinning Service Buckets Multipart Upload API](https://apis.io/collections/filebase/open-filebase-multipart-upload-api/)
- [Filebase IPFS Pinning Service Buckets Node API](https://apis.io/collections/filebase/open-filebase-node-api/)
- [Filebase IPFS Pinning Service Buckets Objects API](https://apis.io/collections/filebase/open-filebase-objects-api/)
- [Filebase IPFS Service Buckets Pinning API](https://apis.io/collections/filebase/open-filebase-pinning-api/)
- [Filebase IPFS Pinning Service Buckets Pins API](https://apis.io/collections/filebase/open-filebase-pins-api/)
- [Filebase IPFS Pinning Service Buckets Usage API](https://apis.io/collections/filebase/open-filebase-usage-api/)

#### Governance rules (1)

Spectral rulesets for the provider's contracts.

- [Filebase — jsonschema rules](https://apis.io/rules/filebase/filebase-jsonschema-spectral-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Filebase Authentication](https://apis.io/security/filebase/filebase-authentication/)
- [Filebase Domain Security](https://apis.io/security/filebase/filebase-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Filebase Plans Pricing](https://apis.io/plans/filebase/filebase-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Filebase Rate Limits](https://apis.io/rate-limits/filebase/filebase-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Filebase Finops](https://apis.io/finops/filebase/filebase-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://filebase.com/)
- [Documentation](https://filebase.com/docs/)
- [Pricing](https://filebase.com/pricing/)
- [Blog](https://filebase.com/blog/)
- [Status](https://status.filebase.com/)

## API Evangelist rating

**Kin Score 32.7** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 71.4 |
| Contract quality | 58.7 |
| Contract governance | 9.8 |
| Operational transparency | 13.2 |
| Developer ergonomics | 23.8 |
| Access clarity | 18.4 |

**Agent readiness 17.9** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
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

**Regulatory alignment 16.7** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/filebase/](https://apis.io/providers/filebase/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Filebase: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/filebase/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
