# Filebase

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
