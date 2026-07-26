# Security Review Questions

## Purpose
This document provides the standard question set used by reviewers when assessing security-related architecture submissions. It is intended to support consistent, evidence-based review outcomes.

## Scope
This guide applies to security review discussions for solution design, change requests, exception requests, and architecture governance checkpoints.

## Required Content
A security review should answer:
- What is being protected?
- What are the trust boundaries?
- Who can access the system?
- How is access granted and revoked?
- How is data protected?
- How are secrets, keys, and credentials managed?
- How are logs and alerts produced?
- What risks remain after controls are applied?

## Review Questions
- What security problem does the design solve?
- What assets are sensitive or regulated?
- Which components are exposed to users, partners, or the internet?
- How is authentication established for each actor?
- Where is authorization enforced?
- Is access limited to the minimum required privilege?
- Are secrets kept out of source code and build artifacts?
- Is data encrypted in transit and at rest?
- Are logs sufficient for detection and investigation?
- Are exceptions documented with compensating controls?
- Is the residual risk acceptable for the bank?

## Evidence
Reviewers should request:
- Security design diagram.
- Identity and access model.
- Network and exposure model.
- Data protection controls.
- Secret and key management controls.
- Logging and monitoring design.
- Threat model or risk assessment.
- Exception approvals where relevant.

## Best Practices
- Ask for evidence before approving the design.
- Use the same core questions across all solutions.
- Record concerns clearly and consistently.
- Escalate gaps that materially increase risk.

## Common Mistakes
- Reviewing only the happy path.
- Accepting vague answers without evidence.
- Treating security as a late-stage checkbox.
- Ignoring cross-cutting impacts on operations and support.

## References
- Security Architecture
- Security Checklist
- Threat Modeling
- MSB security review framework
