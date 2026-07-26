# Secrets Management

## Purpose
This document defines the enterprise guidance for managing secrets, credentials, and sensitive configuration. It helps reviewers ensure that secrets are stored, used, rotated, and audited securely.

## Scope
This guide applies to passwords, API keys, tokens, certificates, private keys, connection strings, and any other secret used by applications, services, administrators, or automation.

## Required Content
Every design should describe:
- Secret types and owners.
- Secret storage location and access model.
- Retrieval and injection mechanism.
- Rotation and expiration strategy.
- Separation between environments.
- Audit logging for access and changes.
- Backup or recovery handling for secret material where applicable.
- Exception handling for legacy or constrained systems.

## Review Questions
- Where are secrets stored?
- Who can read or update each secret?
- Are secrets ever committed to source control or embedded in images?
- How are secrets injected into runtime components?
- Are secrets rotated on a defined schedule or after compromise?
- Are different environments isolated by separate secret namespaces or vaults?
- Is secret access logged and reviewed?
- Are fallback or recovery procedures documented?

## Evidence
Reviewers should request:
- Secret inventory or classification.
- Secret storage architecture.
- Access policy or IAM configuration.
- Rotation procedure or automation evidence.
- Audit log evidence.
- Exception approvals for any hardcoded or transitional secret.

## Best Practices
- Use a centralized secret manager where possible.
- Grant read access only to runtime identities that truly need it.
- Rotate secrets regularly and after incidents.
- Keep secrets out of source code, CI logs, tickets, and documentation examples.
- Separate secrets by environment and sensitivity.
- Prefer short-lived credentials when supported.

## Common Mistakes
- Storing secrets in plain text files or code repositories.
- Reusing one secret across multiple systems.
- Allowing broad access to secret stores.
- Failing to rotate secrets after staff changes or incidents.
- Logging secrets in build, deployment, or application logs.

## References
- Security Architecture
- Authentication and Authorization
- Data Security
- MSB secret handling standards
