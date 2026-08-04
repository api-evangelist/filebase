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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Filebase is an S3-compatible object storage and IPFS pinning platform that combines familiar cloud storage APIs with decentralized, blockchain-backed infrastructure. Developers can store, manage, and pin files to IPFS using standard S3 tooling, a dedicated IPFS Pinning Service API, and an IPFS RPC API — all without changing existing workflows. Filebase delivers geo-redundant 3x replication, free egress for object storage, a global CDN, and predictable pricing.

**Website:** https://filebase.com/  
**Documentation:** https://filebase.com/docs/  
**GitHub:** https://github.com/filebase  
**LinkedIn:** https://www.linkedin.com/company/filebase  
**X:** https://twitter.com/Filebase  
**Blog:** https://filebase.com/blog/  
**Pricing:** https://filebase.com/pricing/  
**Status:** https://status.filebase.com/  

## APIs

| API | Base URL | Description |
|-----|----------|-------------|
| S3-Compatible API | https://s3.filebase.io | Standard S3 protocol for bucket and object management |
| Platform API | https://api.filebase.io | Account-level usage metrics and management |
| IPFS Pinning Service API | https://api.filebase.io/v1/ipfs | Vendor-neutral IPFS pinning standard |
| IPFS RPC API | https://rpc.filebase.io | Core IPFS daemon operations |

## Authentication

- **S3 API:** AWS Signature Version 4 (AWS4-HMAC-SHA256) with access key / secret key pairs
- **Platform API:** HTTP Basic / Bearer token using base64-encoded `<access-key>:<secret-key>`
- **IPFS Pinning Service API:** Per-bucket Bearer token
- **IPFS RPC API:** Bucket-specific Bearer token

## Rate Limits

| API | Limit |
|-----|-------|
| S3-Compatible API | 500 req/s per account |
| Platform API | 500 req/s per account |
| IPFS Pinning Service API | 100 req/s per account |
| IPFS RPC API | 100 req/s per bucket |

## Pricing

| Plan | Price | Storage | IPFS Egress |
|------|-------|---------|-------------|
| Free | $0/mo | 5 GB | 1 GB |
| Pro | $7.50/mo | 500 GB | 250 GB |
| Enterprise | Custom | Custom | Custom |

Object storage egress is free on all plans.

---

*This repository is maintained as part of the [API Evangelist](https://apievangelist.com) APIs.json catalog.*
