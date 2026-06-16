<!-- 
1. Purpose

2. Security Philosophy

3. Secure by Design

4. Authentication Standards

5. Authorization Standards

6. Secrets Management

7. Data Protection

8. API Security

9. Application Security

10. Infrastructure Security

11. Device & IoT Security

12. Supply Chain Security

13. Auditability

14. Incident Response Principles

15. AI Requirements
 -->

# Purpose

The purpose of these standards is to establish security principles that protect:

- Users
- Systems
- Data
- Infrastructure
- Devices
- Business operations

Security must be considered throughout the entire software lifecycle.

Security is not a feature.

Security is a system property.


# Security Philosophy

Security should be designed into systems from the beginning.

Security must support:

- Business continuity
- User trust
- Regulatory compliance
- Operational resilience

Security should enable business growth while managing risk.

Avoid:

- Security by obscurity
- Implicit trust
- Reactive security
- Unverified assumptions


# Secure by Design

Security considerations must be included during:

- Requirements definition
- Architecture design
- Development
- Testing
- Deployment
- Operations

Security should be proactive, not reactive.

Every design should consider:

- Threats
- Attack surfaces
- Failure scenarios
- Abuse scenarios


# Authentication Standards

Every actor must be authenticated.

Actors may include:

- Users
- Services
- Devices
- Applications

Authentication mechanisms must be:

- Verifiable
- Revocable
- Auditable

Avoid anonymous access unless explicitly justified.


# Authorization Standards

Authentication identifies.

Authorization grants permissions.

Apply:

- Least Privilege
- Role-Based Access Control when appropriate
- Explicit permission assignment

Avoid:

- Excessive permissions
- Shared privileged accounts
- Implicit access


# Secrets Management

Secrets must never be stored in source code.

Secrets include:

- Passwords
- API Keys
- Certificates
- Tokens
- Encryption Keys

Secrets must be:

- Rotatable
- Auditable
- Access-controlled

Use centralized secret management solutions whenever possible.


# Data Protection

Data must be protected according to its sensitivity.

Apply:

- Encryption in transit
- Encryption at rest when appropriate
- Data minimization
- Retention policies

Sensitive data should only be accessible to authorized entities.


# API Security

APIs must be protected against unauthorized access and abuse.

Apply:

- Authentication
- Authorization
- Input validation
- Rate limiting when appropriate
- Audit logging

Never trust client-provided data.


# Application Security

Applications should:

- Validate inputs
- Handle errors safely
- Prevent information leakage
- Follow secure coding practices

Security vulnerabilities should be treated as defects.


# Infrastructure Security

Infrastructure should follow:

- Least Privilege
- Network segmentation
- Secure defaults
- Infrastructure as Code when possible

Administrative access should be controlled and auditable.


# Device & IoT Security

Devices must be treated as untrusted until verified.

Apply:

- Device authentication
- Certificate-based trust when possible
- Secure communication channels
- Command authorization

Systems should protect against:

- Device impersonation
- Replay attacks
- Unauthorized commands
- Credential compromise


# Supply Chain Security

Third-party dependencies introduce risk.

Dependencies should be:

- Reviewed
- Maintained
- Monitored

Avoid:

- Unmaintained packages
- Unverified dependencies
- Unnecessary dependencies


# Auditability

Security-relevant actions should be traceable.

Systems should provide audit records for:

- Authentication events
- Authorization changes
- Administrative actions
- Sensitive operations

Audit records should be protected from unauthorized modification.


# Incident Response Principles

Security incidents should be assumed possible.

Systems should support:

- Detection
- Investigation
- Containment
- Recovery

Security events should be observable and actionable.


# AI Requirements

When proposing solutions, always evaluate:

- Authentication requirements
- Authorization requirements
- Data protection needs
- Secrets management implications
- API security implications
- Infrastructure security implications
- Device security implications
- Auditability requirements

Identify potential security risks.

Recommend mitigations.

Recommend ADR creation when security decisions have long-term impact.