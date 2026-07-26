# Availability Architecture

## Purpose
This document defines the enterprise guidance for availability-related architecture review. It helps reviewers assess how a solution is designed to remain reachable and usable when components fail, degrade, or require maintenance.

## Scope
This guide applies to applications, integrations, infrastructure, and supporting services that require defined uptime, failover, or recovery expectations.

## Required Content
Every design should describe:
- Availability target.
- Critical dependencies and failure points.
- Redundancy and failover approach.
- Maintenance strategy.
- Single points of failure.
- Recovery behavior after disruption.
- Availability measurement method.

## Review Questions
- What uptime or service window is required?
- What components are critical to availability?
- Is there any single point of failure?
- How does the solution fail over or recover?
- Can maintenance happen without unacceptable downtime?
- How is availability measured and reported?
- Are dependencies aligned to the same availability target?

## Evidence
Reviewers should request:
- Availability target statement.
- High availability or failover design.
- Dependency map.
- Recovery and maintenance plan.
- Exception approvals for any known availability constraint.

## Best Practices
- Eliminate avoidable single points of failure.
- Design for graceful degradation where full availability is not possible.
- Align dependency availability with the service objective.
- Test failover and recovery paths.

## Common Mistakes
- Defining an uptime target without a supporting design.
- Ignoring external dependencies.
- Assuming manual recovery is fast enough.
- Failing to test failover behavior.

## References
- NFR Architecture
- Resilience Architecture
- Performance Architecture
- MSB availability standards
