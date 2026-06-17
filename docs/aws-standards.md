<!-- 
1. Purpose

2. Cloud Philosophy

3. Account Strategy

4. Identity & Access Management

5. Infrastructure as Code

6. Network Design Principles

7. Secrets Management

8. Compute Standards

9. Data & Storage Standards

10. Observability Standards

11. Cost Management Principles

12. Resilience & Disaster Recovery

13. Deployment Standards

14. Security Governance

15. AI Requirements
 -->

# Purpose

The purpose of these standards is to establish cloud governance principles that ensure:

- Security
- Reliability
- Scalability
- Cost Efficiency
- Operational Excellence

Cloud resources should be managed consistently across all environments and systems.

Cloud architecture should support long-term business growth.


# Cloud Philosophy

Cloud services should be selected based on business and operational needs.

Prioritize:

- Managed services when appropriate
- Operational simplicity
- Reliability
- Security
- Cost efficiency

Avoid:

- Service sprawl
- Unnecessary complexity
- Technology-driven decisions

Cloud architecture should reduce operational burden whenever possible.


# Account Strategy

Cloud environments should be logically isolated.

Separate environments when appropriate:

- Development
- QA
- Production

Access boundaries should be explicit.

Production environments should receive additional protection and governance controls.


# Identity & Access Management

Apply the Principle of Least Privilege.

Access should be:

- Explicit
- Auditable
- Revocable

Avoid:

- Shared accounts
- Excessive permissions
- Permanent elevated access

Identity should be the primary security boundary.


# Infrastructure as Code

Infrastructure should be defined as code whenever possible.

Infrastructure definitions should be:

- Version controlled
- Reviewable
- Reproducible
- Auditable

Manual infrastructure changes should be minimized.


# Network Design Principles

Network boundaries should be intentional.

Apply:

- Segmentation
- Least exposure
- Controlled ingress
- Controlled egress

Public exposure should be justified and documented.

Private communication should be preferred whenever possible.


# Secrets Management

Secrets should be centrally managed.

Secrets must:

- Never be stored in source code
- Be rotatable
- Be access-controlled
- Be auditable

Secrets management should support automation and recovery processes.


# Compute Standards

Compute platforms should be selected according to:

- Business requirements
- Scalability needs
- Operational complexity
- Cost considerations

Prefer managed compute services when operational requirements allow.


# Data & Storage Standards

Data storage should support:

- Durability
- Availability
- Recovery
- Scalability

Data classification should influence storage decisions.

Backup and recovery requirements should be defined for critical systems.


# Observability Standards

Cloud resources should provide operational visibility.

Observability should support:

- Monitoring
- Troubleshooting
- Capacity planning
- Incident response

Operational blind spots should be minimized.


# Cost Management Principles

Cloud spending should be intentional and measurable.

Evaluate:

- Cost efficiency
- Resource utilization
- Scalability costs
- Long-term operational costs

Avoid:

- Unused resources
- Over-provisioning
- Unmonitored spending

Cost should be treated as an architectural concern.


# Resilience & Disaster Recovery

Critical systems should support recovery from failures.

Recovery planning should define:

- Recovery objectives
- Backup strategies
- Failover strategies
- Recovery validation

Recovery capabilities should be periodically tested.


# Deployment Standards

Deployments should be:

- Automated
- Repeatable
- Auditable
- Recoverable

Prefer CI/CD pipelines over manual deployments.

Deployment processes should support rollback strategies.


# Security Governance

Cloud security should align with organizational security standards.

Security controls should be continuously reviewed.

Cloud security decisions with long-term impact should be documented through ADRs.


# AI Requirements

When proposing cloud solutions, always evaluate:

- IAM implications
- Network implications
- Infrastructure requirements
- Cost impact
- Security impact
- Resilience requirements
- Recovery requirements
- Deployment implications
- Observability requirements

Recommend ADR creation for significant cloud architecture decisions.

Prefer managed services when they provide meaningful operational advantages.