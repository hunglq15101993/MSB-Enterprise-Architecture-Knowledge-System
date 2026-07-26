# Threat Modeling

## Purpose
This document defines the enterprise guidance for threat modeling during architecture review. It helps reviewers identify, analyze, and prioritize security risks before implementation.

## Scope
This guide applies to new solutions, major changes, integrations, infrastructure changes, and exception requests where security risks may be introduced or amplified.

## Required Content
Every design should describe:
- Assets and trust boundaries.
- Entry points and attack surfaces.
- Likely threats and abuse cases.
- Existing and proposed controls.
- Residual risk and mitigation plan.
- Open issues requiring review or approval.

## Review Questions
- What are the critical assets?
- What can an attacker reach or influence?
- Which trust boundaries are crossed?
- What are the most likely abuse cases?
- What controls prevent, detect, or respond to those cases?
- Is residual risk acceptable and documented?
- Are high-risk assumptions validated by evidence?

## Evidence
Reviewers should request:
- Threat model diagram or worksheet.
- Data flow diagram.
- Abuse case list.
- Control mapping.
- Risk acceptance or exception record where required.

## Best Practices
- Perform threat modeling early and revisit it when the design changes.
- Focus on realistic abuse scenarios, not only compliance checklists.
- Record mitigations and ownership clearly.
- Use the outcome to drive architecture, testing, and monitoring decisions.

## Common Mistakes
- Treating threat modeling as a one-time formality.
- Ignoring integrations and administrative paths.
- Listing threats without mapping controls.
- Leaving unresolved risks undocumented.

## References
- Security Architecture
- Security Checklist
- Risk Management Guidance
- MSB security review standards
