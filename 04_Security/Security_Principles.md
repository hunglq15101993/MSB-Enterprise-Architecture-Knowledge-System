# Security Principles

## Purpose
This document defines the security principles that govern architecture decisions in the MSB knowledge system. It serves as a baseline for consistent security reasoning across solution reviews.

## Scope
This guide applies to all architecture domains and all solution types that introduce security decisions, exceptions, or compensating controls.

## Required Content
Every security-related design should align with these principles:
- Protect sensitive assets by default.
- Apply least privilege.
- Enforce defense in depth.
- Fail closed when security decisions cannot be confirmed.
- Prefer standard, supportable, and auditable controls.
- Use centralized governance for identity, secrets, and logging where feasible.
- Make exceptions explicit, time-bound, and approved.

## Review Questions
- Which principle is most important in this decision?
- Does the design reduce or increase trust boundaries?
- Is the chosen control standard and supportable?
- Are exceptions documented and approved?
- Is the resulting risk acceptable and traceable?
- Are there compensating controls where ideal controls are not possible?

## Evidence
Reviewers should request:
- Principle-to-decision mapping.
- Exception log or risk acceptance record.
- Supporting design artifacts.
- Approval evidence for non-standard approaches.

## Best Practices
- Use principles as a decision filter, not as slogans.
- Map every exception to a compensating control or risk acceptance.
- Review principles consistently across projects.

## Common Mistakes
- Treating principles as optional.
- Mixing exceptions with standard patterns.
- Allowing undocumented deviations to become normal practice.

## References
- Security Architecture
- Security Checklist
- Security Risk Matrix
- MSB architecture principles and standards
