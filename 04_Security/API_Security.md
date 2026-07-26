# API Security

## Purpose
This document defines the enterprise guidance for securing APIs exposed by MSB solutions. It helps reviewers assess how APIs authenticate callers, enforce authorization, protect payloads, and resist misuse.

## Scope
This guide applies to REST APIs, event-driven interfaces, internal APIs, public APIs, partner APIs, and API gateway or proxy layers that mediate access.

## Required Content
Every API design should describe:
- API exposure model: public, private, internal, or partner.
- Authentication method and trusted identity source.
- Authorization model and scope or permission enforcement.
- Request validation and schema control.
- Rate limiting, throttling, and abuse protection.
- Versioning and backward compatibility strategy.
- Payload size limits and timeout behavior.
- Logging, tracing, and audit requirements.
- Error handling and safe response patterns.

## Review Questions
- Is the API protected by a clear authentication mechanism?
- Are permissions enforced at the API boundary and again in downstream services where needed?
- Are input schemas validated and rejected safely?
- Is the API rate limited or otherwise protected from abuse?
- Are idempotency and replay protections needed?
- Are error responses safe and useful without leaking internals?
- Are public and private APIs separated appropriately?
- Are API logs sufficient for incident investigation?

## Evidence
Reviewers should request:
- API specification or contract.
- Authentication and authorization design.
- Gateway or API management configuration.
- Rate limit and quota policy.
- Example request and response payloads.
- Logging and tracing design.
- Exception approvals for any intentionally exposed endpoint.

## Best Practices
- Protect every non-public API with explicit access control.
- Validate request shape, size, and content.
- Use idempotency keys where repeated calls can cause duplicate effects.
- Rate limit endpoints that are expensive or sensitive.
- Keep internal APIs non-public by default.
- Make authorization decisions observable.

## Common Mistakes
- Exposing internal APIs through convenience routes.
- Relying only on obscurity or non-obvious URLs.
- Failing to set request limits.
- Returning too much detail in API errors.
- Ignoring replay, duplicate submission, or abuse scenarios.

## References
- Security Architecture
- Authentication and Authorization
- Integration Architecture
- MSB API security standards
