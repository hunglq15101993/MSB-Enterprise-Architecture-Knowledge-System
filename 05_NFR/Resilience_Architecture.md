# Resilience Architecture

## Purpose
This document defines the enterprise guidance for resilience-related architecture review. It helps reviewers assess how a solution withstands failures, recovers predictably, and continues to operate under adverse conditions.

## Scope
This guide applies to services, integrations, infrastructure, and operational processes that must tolerate component failures, dependency outages, or partial degradation.

## Required Content
Every design should describe:
- Failure modes and blast radius.
- Resiliency patterns used.
- Retry, timeout, and circuit behavior.
- Recovery objectives.
- Dependency failure handling.
- Data consistency implications.
- Testing and validation approach.

## Review Questions
- What failures are expected and how are they handled?
- How does the system degrade when dependencies fail?
- Are retries, timeouts, and circuit breakers designed safely?
- Can the system recover within the required time?
- Are critical dependencies resilient enough for the target service?
- Is resilience tested with realistic scenarios?

## Evidence
Reviewers should request:
- Resilience design diagram.
- Dependency failure analysis.
- Recovery objectives and test evidence.
- Exception approvals for any unmitigated failure mode.

## Best Practices
- Design for failure rather than assuming stability.
- Keep retry and timeout logic bounded and intentional.
- Prefer graceful degradation over total failure when acceptable.
- Test recovery and failover, not only normal-path operation.

## Common Mistakes
- Retrying indefinitely.
- Ignoring partial outages and degraded states.
- Failing to define recovery behavior.
- Treating resilience as the same thing as availability.

## References
- NFR Architecture
- Availability Architecture
- Performance Architecture
- MSB resilience standards
