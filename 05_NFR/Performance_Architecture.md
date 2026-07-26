# Performance Architecture

## Purpose
This document defines the enterprise guidance for performance-related architecture review. It helps reviewers assess whether a solution can meet required response time, throughput, and resource-efficiency expectations under expected load.

## Scope
This guide applies to applications, integrations, data services, infrastructure, and any component where latency, throughput, or resource consumption affects business outcomes.

## Required Content
Every design should describe:
- Performance objective.
- Workload profile and traffic pattern.
- Response time and throughput target.
- Capacity assumptions.
- Resource bottlenecks and scaling approach.
- Performance testing method.
- Monitoring metrics and thresholds.

## Review Questions
- What latency or throughput target must be met?
- What load profile is expected at peak and steady state?
- What resource limits could constrain the design?
- How does the solution scale under increasing demand?
- How will performance be measured in test and production?
- Are dependencies likely to become bottlenecks?
- Is the target realistic for the chosen architecture?

## Evidence
Reviewers should request:
- Performance target statement.
- Load profile or capacity assumptions.
- Performance test results.
- Scaling and resource design.
- Monitoring metrics and alert thresholds.
- Exception approvals for any untested or relaxed target.

## Best Practices
- Set measurable and business-relevant performance targets.
- Test under realistic data and concurrency conditions.
- Watch for bottlenecks at network, database, and downstream integration layers.
- Scale predictably rather than reactively where possible.

## Common Mistakes
- Defining a target without load assumptions.
- Testing with unrealistic volumes or data shapes.
- Ignoring downstream and shared-service bottlenecks.
- Treating average latency as the only metric.

## References
- NFR Architecture
- Availability Architecture
- Resilience Architecture
- MSB performance standards
