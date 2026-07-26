# Data Security

## Purpose
This document defines the enterprise guidance for protecting data across storage, processing, transmission, backup, and disposal. It helps reviewers assess whether a design is aligned with MSB data protection expectations.

## Scope
This guide applies to customer data, employee data, operational data, logs, reports, analytics outputs, backups, and any other data classified as sensitive or regulated.

## Required Content
Every design should describe:
- Data classification and ownership.
- Sensitive fields and masking requirements.
- Encryption in transit and at rest.
- Access control for data stores and exports.
- Retention, archival, and deletion rules.
- Backup and restore protection.
- Replication and cross-system data movement.
- Audit logging for data access or export.

## Review Questions
- What data classes are stored or processed?
- Are sensitive fields identified explicitly?
- Is the data encrypted at rest and in transit?
- Who can read, update, export, or delete the data?
- Are backups protected to the same standard as primary data?
- Are retention and deletion policies defined?
- Are logs and analytics outputs free of exposed sensitive values?
- Are masking or tokenization controls required anywhere?

## Evidence
Reviewers should request:
- Data classification table.
- Data flow diagram.
- Encryption and key management design.
- Access matrix for data stores and exports.
- Masking or tokenization rules.
- Retention and deletion policy.
- Backup and recovery design.

## Best Practices
- Classify data before designing storage or integration.
- Apply encryption by default.
- Limit direct data store access.
- Mask sensitive values in non-production and reporting use cases.
- Minimize data copied into logs, caches, and temporary files.
- Define deletion and retention controls early.

## Common Mistakes
- Treating all data as non-sensitive.
- Copying production data into lower environments without protection.
- Logging payloads that contain personal or confidential data.
- Leaving exports and extracts uncontrolled.
- Ignoring backup encryption and retention.

## References
- Security Architecture
- Integration Architecture
- Data Architecture
- MSB data protection and privacy standards
