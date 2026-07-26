# Security Risk Matrix

## Purpose
This document defines the standard approach for recording and reviewing security risk in architecture submissions. It helps reviewers compare severity, likelihood, and mitigation status in a consistent way.

## Scope
This guide applies to design reviews, exception requests, threat models, and any architecture decision that introduces or accepts security risk.

## Required Content
Every submission should record:
- Risk description.
- Affected assets and trust boundaries.
- Likelihood and impact assessment.
- Existing controls.
- Proposed mitigations.
- Residual risk.
- Risk owner and target date.
- Approval or escalation path.

## Review Questions
- What is the risk and what causes it?
- Which assets or processes are impacted?
- How severe is the impact if the risk materializes?
- How likely is the risk to occur?
- What controls reduce the likelihood or impact?
- Is the remaining risk acceptable to the bank?
- Who owns the risk and the mitigation timeline?

## Evidence
Reviewers should request:
- Risk register entry or equivalent.
- Threat model or issue analysis.
- Control mapping.
- Mitigation plan.
- Risk acceptance or exception approval where needed.

## Best Practices
- Record risks early and update them when the design changes.
- Use consistent severity and likelihood definitions.
- Tie each risk to a concrete owner and action.
- Escalate unresolved high risks.

## Common Mistakes
- Describing risks vaguely.
- Missing ownership or due dates.
- Ignoring residual risk after controls are added.
- Treating mitigation as complete without evidence.

## References
- Security Architecture
- Threat Modeling
- Security Review Questions
- MSB risk management standards
