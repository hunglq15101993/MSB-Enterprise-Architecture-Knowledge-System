# Identity and Access Management

## Purpose
This document defines the enterprise guidance for identity and access management in architecture review. It helps reviewers assess how identities are established, governed, and protected across people, applications, and services.

## Scope
This guide applies to employee access, privileged administration, application identities, service accounts, partner access, and any federated or delegated identity model.

## Required Content
Every design should describe:
- Identity source and trust boundary.
- User, service, and admin identity types.
- Authentication and federation approach.
- Authorization model and permission governance.
- Joiner, mover, and leaver process.
- Privileged access workflow.
- Access review and recertification approach.
- Audit trail for identity lifecycle events.

## Review Questions
- What is the authoritative identity source?
- How are identities provisioned and deprovisioned?
- How are privileged roles approved and reviewed?
- Are service accounts uniquely owned and controlled?
- Are shared or generic accounts avoided?
- Are access reviews performed on a defined schedule?
- Is identity data protected and audited?
- Can the design explain who has access and why?

## Evidence
Reviewers should request:
- Identity architecture diagram.
- Access provisioning and deprovisioning workflow.
- Role and group model.
- Privileged access process.
- Access review evidence.
- Exception approvals for any shared or legacy account.

## Best Practices
- Use centralized identity governance.
- Separate user, admin, and service identities.
- Grant access through roles or groups rather than direct ad hoc assignment where possible.
- Review access regularly and remove stale permissions.
- Limit shared accounts and compensate with stronger controls when unavoidable.

## Common Mistakes
- Leaving orphaned accounts active.
- Using shared credentials for convenience.
- Failing to recertify privileged access.
- Granting direct permissions without traceable ownership.
- Ignoring service account lifecycle management.

## References
- Authentication and Authorization
- Security Architecture
- BAR Governance
- MSB identity governance standards
