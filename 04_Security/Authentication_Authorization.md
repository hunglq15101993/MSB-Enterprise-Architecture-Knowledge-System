# Authentication and Authorization

## Purpose
This document defines the enterprise guidance for authentication and authorization across MSB architecture reviews. It standardizes how identity is established, how access is granted, and how privileged actions are controlled.

## Scope
This guide applies to human users, service accounts, applications, APIs, administrative consoles, batch jobs, and machine-to-machine communication. It is relevant to all architecture domains where access control decisions affect security or compliance.

## Required Content
Every solution should describe:
- Identity provider or trust source.
- Authentication method for each actor type.
- Authorization model and policy enforcement points.
- Token type, lifetime, renewal, and revocation approach.
- Role, group, claim, or permission mapping.
- Privileged access and administrative controls.
- Service-to-service authentication approach.
- Session handling and logout behavior.
- Audit trail for authentication and access decisions.

## Authentication Principles
- Authenticate each actor before access is granted.
- Use centralized identity where possible.
- Prefer standards-based protocols such as SSO, OAuth2, OIDC, SAML, or mutually authenticated service channels where appropriate.
- Avoid custom authentication logic unless there is a documented bank-approved reason.
- Treat session and token handling as security-sensitive design elements.

## Authorization Principles
- Enforce least privilege.
- Apply authorization at every relevant trust boundary.
- Separate coarse-grained and fine-grained access control where needed.
- Use explicit deny or fail-closed behavior for protected actions.
- Make authorization decisions traceable in logs and review evidence.

## Review Questions
- How is the user, service, or system authenticated?
- What identity provider is trusted?
- Are passwords, tokens, certificates, or assertions handled securely?
- How are roles and permissions mapped?
- Where is authorization enforced: gateway, API, service, or data layer?
- Are privileged functions protected with stronger controls?
- Are session timeout, refresh, revocation, and logout defined?
- Are machine-to-machine credentials rotated and audited?
- Can the design prove who accessed what and when?

## Evidence
Reviewers should request:
- Identity architecture diagram.
- Authentication flow diagram.
- Authorization matrix or access model.
- Token and session lifecycle design.
- SSO or federation configuration details.
- Administrative access model.
- Audit logging evidence.
- Exception approvals for any non-standard access pattern.

## Best Practices
- Centralize identity when possible.
- Use short-lived credentials for privileged or machine access.
- Separate authentication from authorization concerns.
- Validate tokens and assertions at trusted boundaries.
- Recheck permissions for sensitive or destructive operations.
- Review access grants periodically.

## Common Mistakes
- Mixing authentication code with business logic.
- Hardcoding access rules in multiple services without governance.
- Using long-lived tokens without refresh or revocation strategy.
- Granting broad admin roles for convenience.
- Failing to log access decisions.
- Assuming front-end checks are sufficient for protection.

## References
- Security Architecture
- BAR Governance
- Architecture Review Questions
- MSB identity and access standards
