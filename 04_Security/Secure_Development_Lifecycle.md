# Secure Development Lifecycle

## Purpose
This document defines the enterprise guidance for incorporating security into the development lifecycle. It helps reviewers confirm that security is considered from design through delivery and operation.

## Scope
This guide applies to project initiation, design, implementation, testing, release, and post-release maintenance for MSB solutions.

## Required Content
Every delivery approach should describe:
- Security requirements capture.
- Threat modeling or risk analysis.
- Secure coding practices.
- Dependency and vulnerability management.
- Security testing and review gates.
- Release approval criteria.
- Incident response and post-release remediation.

## Review Questions
- Are security requirements defined before implementation starts?
- Is threat modeling performed for material changes?
- Are secure coding standards enforced?
- Are vulnerabilities scanned and tracked to closure?
- Are release gates defined for security findings?
- Are exceptions approved and time-bound?
- Is there a plan for post-release security maintenance?

## Evidence
Reviewers should request:
- Secure SDLC process or policy.
- Threat model or design review evidence.
- Vulnerability scanning results.
- Security test results.
- Release gate or approval checklist.
- Exception records where needed.

## Best Practices
- Treat security as a non-functional requirement from the start.
- Build security review into each delivery milestone.
- Make remediation ownership explicit.
- Use automated checks where practical.

## Common Mistakes
- Addressing security only at the end of the project.
- Releasing with known high-risk findings without approval.
- Treating scanning as a replacement for design review.
- Losing track of remediation ownership.

## References
- Security Architecture
- Threat Modeling
- Security Checklist
- MSB SDLC standards
