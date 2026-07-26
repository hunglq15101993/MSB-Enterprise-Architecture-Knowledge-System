# Security Controls

## Purpose
This document defines the security control baseline used in architecture reviews. It helps reviewers identify whether the proposed solution includes the right preventive, detective, and corrective controls.

## Scope
This guide applies to controls across identity, network, application, data, operations, monitoring, and exception handling.

## Required Content
Every design should describe:
- Preventive controls.
- Detective controls.
- Corrective or recovery controls.
- Control ownership.
- Control evidence.
- Control gaps and compensating controls.
- Control testing or validation approach.

## Review Questions
- Which security controls are mandatory for this solution?
- Are the controls preventive, detective, or corrective?
- Who owns each control?
- How will control effectiveness be proven?
- Are there gaps that require compensation?
- Are controls aligned with the identified risks?
- Are control failures observable and actionable?

## Evidence
Reviewers should request:
- Control matrix.
- Test or validation evidence.
- Operational ownership mapping.
- Exception approvals for missing or partial controls.

## Best Practices
- Map controls to concrete risks.
- Prefer controls that are measurable and testable.
- Keep ownership explicit.
- Revalidate controls after major changes.

## Common Mistakes
- Listing controls without explaining why they exist.
- Over-relying on a single control for a critical risk.
- Failing to test whether a control actually works.
- Leaving ownership unclear.

## References
- Security Architecture
- Security Risk Matrix
- Threat Modeling
- MSB control standards
