# Network Security

## Purpose
This document defines the enterprise guidance for network security review in MSB architecture. It helps reviewers assess how systems are segmented, protected, and exposed across internal, external, and third-party connectivity.

## Scope
This guide applies to cloud, on-premises, hybrid, DMZ, API exposure, service-to-service traffic, remote access, and any design that crosses a trust boundary or network segment.

## Required Content
Every design should describe:
- Network zones and trust boundaries.
- Ingress and egress paths.
- Public, private, and internal endpoints.
- Security groups, firewall rules, and routing controls.
- TLS termination and encryption in transit.
- VPN, private link, peering, or dedicated connectivity where applicable.
- WAF, gateway, proxy, or inspection layers.
- DDoS or abuse protection where relevant.
- Network exceptions and compensating controls.

## Review Questions
- What networks can reach the workload?
- Is the service publicly exposed, or only reachable privately?
- Are inbound and outbound connections restricted to required destinations?
- Is traffic encrypted in transit?
- Are trust boundaries clearly documented?
- Is there an inspection or protection layer for internet-facing traffic?
- Are administrative paths isolated from application traffic?
- Are route tables, firewall rules, and security groups aligned with the intended design?

## Evidence
Reviewers should request:
- Network topology diagram.
- Ingress and egress matrix.
- Firewall, security group, or network policy configuration.
- TLS configuration details.
- WAF, proxy, or load balancer design.
- Private connectivity design where applicable.
- Exception approvals for open or shared paths.

## Best Practices
- Minimize public exposure.
- Default deny on inbound and outbound access.
- Separate administrative and application traffic.
- Use private connectivity for sensitive integrations.
- Segment workloads by function and sensitivity.
- Protect internet-facing endpoints with inspection or edge controls.

## Common Mistakes
- Exposing services publicly without business need.
- Allowing broad east-west traffic between tiers.
- Mixing admin and user traffic in the same path.
- Documenting firewall rules without explaining why they exist.
- Ignoring egress control and third-party destinations.

## References
- Security Architecture
- Deployment Architecture
- Integration Architecture
- MSB network and perimeter standards
