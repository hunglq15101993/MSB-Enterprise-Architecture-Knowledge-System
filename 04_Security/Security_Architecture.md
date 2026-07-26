# Security Architecture

## Purpose
This document defines the security architecture baseline for the MSB Enterprise Architecture Knowledge System. It provides a consistent reference for designing, reviewing, and governing security controls across business, application, integration, data, deployment, and technology domains.

## Scope
This guide applies to all architecture review activities that involve identity, access, network, application, data, secrets, logging, monitoring, and secure operations. It is intended for Enterprise Architects, Solution Architects, Technical Architects, BAR reviewers, and Lead Engineers.

## Security Objectives
- Protect customer, employee, and bank data.
- Enforce strong identity and access control.
- Reduce attack surface across all layers.
- Support regulatory, audit, and governance expectations.
- Provide traceable evidence for architecture decisions.

## Required Content
Each security design or review submission should describe:
- Security objective and business risk addressed.
- Trust boundaries and sensitive assets.
- Authentication and authorization model.
- Network segmentation and traffic protection.
- Data protection controls for storage, transit, and backup.
- Secret and key management approach.
- Logging, monitoring, and alerting strategy.
- Vulnerability management and secure delivery practices.
- Exceptions, compensating controls, and residual risks.

## Security Domains
### Identity and Access Management
Define how users, services, and administrators authenticate and how permissions are granted, reviewed, and revoked.

### Network Security
Describe segmentation, firewall rules, TLS enforcement, private connectivity, ingress and egress control, and perimeter protection.

### Application Security
Cover input validation, session handling, secure headers, dependency control, token handling, and abuse prevention.

### Data Security
Explain data classification, encryption, masking, retention, deletion, and backup protection.

### Secrets and Key Management
Define how secrets are stored, rotated, accessed, and audited. Include KMS/HSM or equivalent enterprise controls where applicable.

### Logging and Monitoring
Explain which events are collected, where they are stored, how they are protected, and how anomalies are detected and escalated.

## Review Questions
- What security risks are introduced by this design?
- What are the trust boundaries?
- How is authentication performed?
- How is authorization enforced at each layer?
- Is least privilege applied to users and services?
- Is data encrypted in transit and at rest?
- Are secrets removed from code and configuration files?
- Are logs sufficient for detection and investigation without exposing sensitive data?
- What compensating controls exist for unresolved risks?

## Evidence
Reviewers should request evidence such as:
- Security architecture diagram.
- Identity and access model.
- Firewall, WAF, or network policy configuration.
- Encryption and key management design.
- Secret management design.
- Logging and monitoring design.
- Threat analysis or risk assessment.
- Exceptions and approvals for non-standard patterns.

## Best Practices
- Use defense in depth.
- Apply least privilege by default.
- Separate duties for development, operations, and approval.
- Prefer managed security services where appropriate.
- Centralize logging and make logs tamper resistant.
- Treat credentials, tokens, and keys as high sensitivity assets.
- Use secure defaults and remove unused access paths.

## Common Mistakes
- Assuming perimeter security is sufficient.
- Storing secrets in source code or plain text configuration.
- Granting broad access to simplify implementation.
- Encrypting data but ignoring access control.
- Logging sensitive payloads without redaction.
- Leaving exceptions undocumented and unaudited.

## Review Questions for BAR
- Does the solution align with bank security policies?
- Are all critical assets classified and protected?
- Are authentication and authorization controls explicit and testable?
- Are there any policy exceptions requiring formal approval?
- Is the residual risk acceptable for production use?

## References
- Enterprise Architecture Review Framework
- Evidence Policy
- Confidence Model
- Output Standard
- MSB security policy and applicable bank standards
