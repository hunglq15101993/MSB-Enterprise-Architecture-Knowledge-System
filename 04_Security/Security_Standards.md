# Security Standards

## Purpose
This document defines the standards baseline referenced by security architecture reviews. It helps reviewers confirm that proposed designs align with approved bank standards rather than ad hoc practice.

## Scope
This guide applies to any solution, platform, integration, or operational process that depends on security requirements, exceptions, or control validation.

## Required Content
Every design should describe:
- Applicable internal standards.
- Applicable external or regulatory standards if relevant.
- Control expectations by domain.
- Evidence required for compliance.
- Exception handling and approval.
- Ownership for standard interpretation.

## Review Questions
- Which standards apply to this solution?
- Are the required controls explicitly mapped?
- Are there any deviations from standard?
- Who approves exceptions?
- Is the design using approved patterns or products?
- Is evidence sufficient to prove compliance?
- Are standards updated when the architecture changes?

## Evidence
Reviewers should request:
- Standards mapping matrix.
- Exception requests and approvals.
- Supporting design artifacts.
- Operational evidence where required.

## Best Practices
- Maintain a clear mapping from standards to architecture decisions.
- Keep exception handling formal and time-bound.
- Use approved standards as the first design option.

## Common Mistakes
- Assuming an exception is approved because it is documented informally.
- Applying standards inconsistently across teams.
- Referencing standards without proving implementation.

## References
- Security Architecture
- Security Controls
- Security Checklist
- MSB security standards catalog
