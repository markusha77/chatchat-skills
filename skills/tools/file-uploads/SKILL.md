---
id: file-uploads
name: File Uploads
description: Design and troubleshoot secure, reliable file upload flows across clients, APIs, storage, validation, and post-upload processing.
category: Tools
requires: []
examples:
  - "Implement a presigned upload flow with server-side validation and malware scanning hooks."
  - "Debug intermittent large-file upload failures caused by timeout or multipart misconfiguration."
---

# File Uploads

Use this skill to design, review, or debug file upload flows that need to be secure, reliable, and understandable across frontend, API, storage, and background processing.

## Clarify First
- What kinds of files are allowed and why.
- Which trust boundaries exist between client, API, storage, and processing systems.
- Whether uploads are small, large, resumable, high-volume, or latency-sensitive.
- Which validations must happen before a file becomes usable.
- What happens after upload: scanning, indexing, transformation, or review.

## Core Design Choices
- Direct-to-storage versus proxy-through-API versus hybrid handoff.
- Single-request versus multipart or chunked upload strategy.
- Private-by-default storage versus deliberate public access.
- Immediate versus asynchronous post-upload processing.
- Strict validation at one layer versus defense in depth across layers.

## Good Upload Guidance
- Keep credentials and write authority off the client whenever possible.
- Validate size, type, and ownership explicitly.
- Treat integrity and retry behavior as first-class design concerns.
- Separate upload success from post-processing success.
- Instrument each phase so failures are easy to localize.

## Failure Modes To Look For
- Browser or mobile clients timing out on large transfers.
- Trusting client-provided MIME type or filename alone.
- Orphaned multipart state after failed uploads.
- Publicly accessible objects created before validation or scanning is complete.
- CORS or auth mismatches that block otherwise valid upload flows.

## What To Surface
- Recommended upload architecture and trust boundaries.
- Validation and hardening controls in rollout order.
- Likely failure points by phase: auth, transfer, validation, processing.
- Observability gaps that make upload incidents hard to debug.
- Concrete implementation choices such as expiry windows, part sizes, or cleanup approach.

## Common Mistakes
- Using silent defaults that accept file types or sizes too broadly.
- Treating upload completion as proof the file is safe or usable.
- Letting clients hold long-lived write credentials.
- Ignoring retry, resumability, and cleanup behavior until production failures appear.
- Designing the happy path only and skipping weak-network conditions.

## Boundaries
- Do not present example architectures as already implemented unless the user confirms them.
- Prefer guidance on validation, trust boundaries, and failure analysis over implying direct access to storage or upload infrastructure.
