# Compliance and Privacy

## Purpose
This document defines the enterprise guidance for security-related compliance and privacy considerations in architecture review. It helps reviewers verify that the solution respects legal, regulatory, and internal policy obligations.

## Scope
This guide applies to any design that collects, processes, stores, transmits, or reports personal, confidential, or regulated information.

## Required Content
Every design should describe:
- Applicable compliance obligations.
- Privacy-sensitive data categories.
- Lawful basis or policy basis for processing where relevant.
- Data minimization and purpose limitation.
- Consent, notice, or disclosure requirements where applicable.
- Retention and deletion obligations.
- Cross-border transfer or residency constraints.
- Audit and evidence requirements.

## Review Questions
- What compliance or privacy obligations apply to this solution?
- Are sensitive or regulated data types identified clearly?
- Is collection limited to the minimum necessary?
- Are retention and deletion rules documented?
- Are cross-border or third-party transfers allowed?
- Are access and logging controls sufficient for auditability?
- Are privacy risks and exceptions documented?
- Are owners responsible for monitoring ongoing compliance?

## Evidence
Reviewers should request:
- Data classification and privacy impact assessment where required.
- Retention and deletion policy.
- Data transfer or residency design.
- Audit evidence or logging design.
- Approval records for any exception or non-standard processing.

## Best Practices
- Identify compliance and privacy obligations early.
- Minimize collection and retention.
- Restrict access to need-to-know.
- Document transfers, disclosures, and exceptions.
- Keep evidence ready for internal review and audit.

## Common Mistakes
- Treating privacy as a downstream operational issue.
- Keeping sensitive data longer than necessary.
- Allowing uncontrolled exports or transfers.
- Failing to document exception approvals.

## References
- Security Architecture
- Data Security
- Security Risk Matrix
- MSB compliance and privacy standards
