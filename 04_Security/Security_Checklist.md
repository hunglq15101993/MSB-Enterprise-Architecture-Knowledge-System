# Security Checklist

## Purpose
This checklist provides a concise review aid for security-related architecture submissions. It helps reviewers verify that the most important security topics have been addressed before approval.

## Scope
This checklist applies to architecture reviews, design reviews, change requests, and exception assessments involving MSB systems or integrations.

## Checklist
- Identity source is defined.
- Authentication method is defined for each actor type.
- Authorization model is explicit.
- Least privilege is applied.
- Network exposure is minimized.
- Sensitive data is encrypted in transit and at rest.
- Secrets are not embedded in code or plain text config.
- Logging and monitoring are defined.
- Security exceptions are documented and approved.
- Residual risk is stated clearly.

## Review Questions
- Is there a clear security owner?
- Are trust boundaries documented?
- Are public and private endpoints justified?
- Is admin access separated from end-user access?
- Are sensitive logs or payloads redacted?
- Are keys, tokens, and credentials managed securely?
- Is there evidence for the stated controls?
- Are any gaps called out with compensating controls?

## Evidence
- Security architecture diagram.
- Access matrix.
- Network diagram.
- Encryption and secrets design.
- Logging and monitoring plan.
- Exception log and approvals.

## Best Practices
- Use this checklist early, not only at final review.
- Treat missing evidence as a review blocker when the risk is material.
- Keep checklist answers short, direct, and evidence-based.

## Common Mistakes
- Copying checklist answers from another solution.
- Marking items complete without evidence.
- Ignoring exceptions that should have been escalated.

## References
- Security Architecture
- Authentication and Authorization
- Data Security
- Logging and Monitoring
