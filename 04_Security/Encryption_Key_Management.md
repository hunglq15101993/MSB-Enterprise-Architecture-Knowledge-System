# Encryption and Key Management

## Purpose
This document defines the enterprise guidance for encryption and key management. It helps reviewers ensure that sensitive information is protected using approved cryptographic controls and governed key lifecycles.

## Scope
This guide applies to encryption in transit, encryption at rest, application-level encryption, key generation, key storage, rotation, revocation, and any cryptographic dependency used by bank solutions.

## Required Content
Every design should describe:
- What data or traffic is encrypted.
- Which algorithms, protocols, or approved services are used.
- Who owns the keys.
- Where keys are stored and protected.
- Rotation, expiration, and revocation policy.
- Certificate lifecycle management where relevant.
- Separation of duties for key administration.
- Exception handling for legacy or constrained systems.

## Review Questions
- What is encrypted and why?
- Are approved cryptographic standards being used?
- Where are keys or certificates stored?
- Who can administer or retrieve them?
- How often are they rotated?
- Are expired or revoked keys handled safely?
- Are encryption boundaries clear across network, storage, and application layers?
- Is any custom crypto design involved?

## Evidence
Reviewers should request:
- Encryption architecture diagram.
- Key ownership and access model.
- Certificate lifecycle details.
- Rotation or revocation procedure.
- KMS, HSM, or approved cryptographic service configuration.
- Exception approvals for non-standard algorithms or legacy constraints.

## Best Practices
- Prefer approved enterprise cryptographic services.
- Use encryption in transit by default.
- Use encryption at rest for sensitive data stores and backups.
- Separate key administration from application runtime access.
- Rotate keys and certificates on a defined schedule.
- Avoid custom crypto implementations.

## Common Mistakes
- Using outdated or unapproved algorithms.
- Hardcoding key material in code or configuration.
- Ignoring certificate expiry.
- Encrypting data without managing the keys properly.
- Reusing keys across unrelated systems or environments.

## References
- Security Architecture
- Data Security
- Secrets Management
- MSB cryptography standards
