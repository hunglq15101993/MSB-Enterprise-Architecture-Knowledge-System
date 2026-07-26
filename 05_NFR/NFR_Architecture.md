# Non-Functional Requirements (NFR) Architecture

## Purpose
This document defines the enterprise guidance for non-functional requirements in architecture review. It helps reviewers assess whether a solution can meet required levels of performance, availability, scalability, resilience, maintainability, and operability.

## Scope
This guide applies to all solutions, integrations, platforms, and infrastructure components that introduce quality-of-service expectations or operational constraints.

## Required Content
Every design should describe:
- NFR categories that apply.
- Expected service levels.
- Measurement method and metrics.
- Assumptions and capacity drivers.
- Operational dependencies.
- Risks, constraints, and trade-offs.
- Validation and testing approach.

## Review Questions
- Which NFRs are mandatory for this solution?
- What is the target performance, availability, and resilience level?
- How will the solution be measured in production?
- Are there peak load or growth assumptions?
- What operational constraints could reduce NFR achievement?
- Are there trade-offs between cost, complexity, and quality?
- Can the design prove the NFRs with evidence?

## Evidence
Reviewers should request:
- NFR statement or matrix.
- Capacity assumptions.
- Performance and resilience test evidence.
- Monitoring and alerting design.
- Recovery and failover approach.
- Exception approvals for any non-standard target.

## Best Practices
- Define NFRs early and make them measurable.
- Tie each NFR to a business outcome.
- Validate important NFRs before production.
- Track operational metrics continuously.

## Common Mistakes
- Leaving NFRs vague or unmeasured.
- Treating NFRs as purely technical preferences.
- Ignoring dependencies that affect availability or latency.
- Approving a design without evidence.

## References
- Availability Architecture
- Performance Architecture
- Resilience Architecture
- MSB NFR standards
