# Security Logging and Monitoring

## Purpose
This document defines the enterprise guidance for logging and monitoring security-relevant activity. It helps reviewers assess whether a solution produces usable evidence for detection, investigation, and governance.

## Scope
This guide applies to application logs, security logs, audit logs, access logs, infrastructure logs, admin activity, alerting, dashboards, and any monitoring control used to detect security events.

## Required Content
Every design should describe:
- Security events that must be logged.
- Log destinations and retention.
- Access control and protection for log data.
- Correlation identifiers and traceability.
- Alerting thresholds and escalation paths.
- Detection use cases for abuse or compromise.
- Log redaction and sensitive-data handling.
- Audit evidence for administrative or privileged actions.

## Review Questions
- Which events are captured as security-relevant?
- Are logs centralized and protected from tampering?
- Can reviewers trace an action from user entry point to backend effect?
- Are alerts defined for suspicious or high-risk activity?
- Are sensitive fields masked or excluded from logs?
- Are log retention and archival periods defined?
- Can administrators access logs without creating excessive risk?
- Are monitoring dependencies and failure modes documented?

## Evidence
Reviewers should request:
- Logging and monitoring architecture diagram.
- List of security events collected.
- Log retention and access policy.
- Alert definitions or SIEM use cases.
- Redaction or masking rules.
- Sample audit trails for sensitive actions.

## Best Practices
- Centralize logs where possible.
- Correlate events across application, identity, network, and infrastructure layers.
- Protect logs from deletion and unauthorized modification.
- Alert on privileged actions and unusual access patterns.
- Exclude or mask sensitive values.
- Define operational ownership for monitoring and incident response.

## Common Mistakes
- Logging too little to investigate incidents.
- Logging too much sensitive information.
- Leaving logs on local disks without protection.
- Failing to correlate events across systems.
- Creating alerts that are not actionable.

## References
- Security Architecture
- Authentication and Authorization
- Data Security
- MSB logging and monitoring standards
