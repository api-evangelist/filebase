<!-- fetched 2026-10-13 from https://docs.filebase.com/api-documentation/s3-compatible-api by sweep-shape-compat.py; text extracted from the provider's own page -->

S3 API overview | Filebase Docs Skip to main content 
 Documentation S3 API SDKs 
 Blog Pricing Console 
 Introduction 
 Get started 
 Sign up 
 Create a bucket 
 Access keys 
 AWS CLI quickstart 
 AWS SDK (JavaScript) 
 AWS SDK (Python) 
 AWS SDK (Go) 
 Core concepts 
 Account & billing 
 S3 API 
 Overview 
 Authentication 
 Supported operations 
 Multipart upload 
 Pre-signed URLs 
 CORS 
 Server-side encryption 
 Object checksums 
 Error codes 
 Rate limits 
 S3 compatibility matrix 
 Platform API 
 SDKs 
 Frameworks 
 CLI tools 
 Desktop & mobile clients 
 Backup software 
 NAS & storage 
 CDN integrations 
 Kubernetes 
 Recipes 
 IPFS 
 S3 API 
 On this page 
 S3 API overview
 The Filebase S3 API implements the same operations as AWS S3 — PutObject , GetObject , ListObjectsV2 , multipart upload, pre-signed URLs, CORS, and the rest. Any S3-compatible client, SDK, framework integration, or third-party tool that targets AWS S3 can target Filebase by changing two values.
 Endpoint ​ 
 https://s3.filebase.io 
 This single endpoint serves every Filebase bucket, globally. Filebase does not expose per-region endpoints — bucket access is routed transparently by the Filebase CDN .
 HTTP requests are redirected to HTTPS on port 443. There is no plaintext endpoint and no way to opt out.
 Region ​ 
 auto 
 Use the literal string auto . The AWS SDKs require a region value to compute the SigV4 signing key — auto satisfies that requirement and tells Filebase to route to whichever backend serves the bucket.
 If your tool or SDK rejects auto as a region (rare — most accept any non-empty string), use us-east-1 as a fallback.
 Authentication ​ 
 Every authenticated request is signed with AWS Signature Version 4 ( AWS4-HMAC-SHA256 ). Filebase does not accept SigV2.
 You don't write the signing logic yourself — every modern S3 client does it for you. You just supply the access key pair via standard mechanisms:
 AWS CLI: aws configure 
 SDKs: a credentials block in the client constructor
 Environment variables: AWS_ACCESS_KEY_ID , AWS_SECRET_ACCESS_KEY 
 See authentication for the full reference.
 Addressing styles ​ 
 Filebase supports both addressing styles — use whichever your SDK or tool defaults to:
 https://s3.filebase.io/<bucket-name>/<object-key> ✓ path style 
 https://<bucket-name>.s3.filebase.io/<object-key> ✓ virtual-host style 
 You don't need to set any path-style flag ( forcePathStyle , addressing_style , UsePathStyle , etc.) — leave the SDK at its default. Both styles are signed and served identically.
 For anonymous reads from public buckets, use the virtual-host style URL: https://<bucket>.s3.filebase.io/<key> . This is the URL the Filebase CDN serves, and it's what you'd embed in a website or email out.
 Supported operations ​ 
 See the supported operations reference for the full list and the compatibility matrix for the precise behavior of each.
 The most-used operations:
 Object lifecycle: PutObject , GetObject , HeadObject , DeleteObject , CopyObject 
 Listing: ListObjectsV2 , ListObjects 
 Buckets: CreateBucket , DeleteBucket , HeadBucket , ListBuckets , GetBucketLocation 
 Multipart upload: CreateMultipartUpload , UploadPart , CompleteMultipartUpload , AbortMultipartUpload 
 ACL: GetBucketAcl , PutBucketAcl , GetObjectAcl (returns the bucket ACL)
 CORS: GetBucketCors , PutBucketCors , DeleteBucketCors 
 Lifecycle: GetBucketLifecycle , GetBucketLifecycleConfiguration 
 Versioning: GetBucketVersioning 
 Logging: GetBucketLogging 
 Operation classes ​ 
 Each successful S3 API request is billed as Class A , Class B , or free . See pricing for rates, free-tier inclusions, and worked examples.
 Class A operations ​ 
 State-mutating — writes and configuration changes.
 ListBuckets , PutBucket , ListObjects , PutObject , CopyObject , CompleteMultipartUpload , CreateMultipartUpload , ListMultipartUploads , UploadPart , ListParts , PutBucketEncryption , PutBucketCors .
 Class B operations ​ 
 State-reading — non-mutating reads of objects, metadata, or configuration.
 HeadBucket , HeadObject , GetObject , GetBucketEncryption , GetBucketLocation , GetBucketCors , GetBucketLifecycleConfiguration .
 Free operations ​ 
 Never billed, on any plan.
 DeleteObject , DeleteBucket , AbortMultipartUpload .
 Response format ​ 
 When a response has a body, it's returned as UTF-8 encoded XML — same as AWS S3. Error responses follow the standard S3 error schema (Code, Message, Resource, RequestId).
 Rate limit ​ 
 500 requests per second per account. See rate limits .
 What's next ​ 
 Authentication 
 Supported operations 
 Compatibility matrix 
 Pre-signed URLs 
 Multipart upload 
 Migrating from AWS S3 
 Previous
 Closing your account
 Next
 Overview
 Endpoint 
 Region 
 Authentication 
 Addressing styles 
 Supported operations 
 Operation classes Class A operations 
 Class B operations 
 Free operations 
 Response format 
 Rate limit 
 What's next 
 Company
 About 
 Blog 
 Resources
 Pricing 
 Terms of Service 
 Privacy Policy 
 Documentation
 Get Started 
 S3 API Reference 
 SDKs 
 Migrating from AWS S3 
 Support
 Email support 
 Discord 
 GitHub 
 Copyright © 2026 Filebase, Inc.
