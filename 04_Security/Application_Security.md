# Application Security

## Purpose
This document defines the enterprise guidance for reviewing security controls implemented within applications. It helps reviewers assess whether the application layer resists common attack patterns and protects sensitive functions.

## Scope
This guide applies to web applications, APIs, back-end services, front-end clients, batch services, and shared libraries where application logic can introduce security risk.

## Required Content
Every application design should describe:
- Input validation and output encoding.
- Authentication and authorization enforcement points.
- Session and token handling.
- Secure error handling and response behavior.
- Dependency and library governance.
- Protection against abuse, replay, and tampering.
- CSRF, XSS, SSRF, injection, and deserialization considerations where relevant.
- Logging and monitoring of security-relevant events.

## Review Questions
- How does the application validate input and protect output?
- Are security checks enforced on the server side?
- Are sessions, cookies, or tokens handled securely?
- Are sensitive actions protected against replay or abuse?
- Are secrets, credentials, or sensitive values exposed in code or logs?
- Are vulnerable dependencies scanned and governed?
- Are error messages safe for production?
- Are security assumptions documented and testable?

## Evidence
Reviewers should request:
- Application security architecture diagram.
- Secure coding standards or guidelines.
- Dependency and vulnerability scanning evidence.
- Token/session handling design.
- Security test cases or penetration findings where available.
- Exception approvals for any intentional deviation.

## Best Practices
- Validate all inputs at trust boundaries.
- Fail safely and avoid exposing internals.
- Prefer server-side authorization checks.
- Keep secrets out of source code and client-side storage where possible.
- Use framework security features intentionally and consistently.
- Scan dependencies and patch known issues promptly.

## Common Mistakes
- Trusting client-side validation alone.
- Returning detailed stack traces or internal errors to users.
- Implementing custom crypto or custom security protocols.
- Ignoring dependency vulnerabilities.
- Storing sensitive data in logs, local storage, or cookies without justification.

## References
- Security Architecture
- Authentication and Authorization
- API Security
- MSB secure coding standards
