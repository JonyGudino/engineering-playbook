<!-- 
1. Purpose

2. Design Philosophy

3. Domain Design Principles

4. Service Design Principles

5. Data Design Principles

6. Integration Principles

7. Reliability Principles

8. Scalability Principles

9. Security Principles

10. Observability Principles

11. Evolution Principles

12. AI Requirements
 -->

# Purpose

The purpose of these principles is to guide the design of software systems that are:

- Maintainable
- Reliable
- Scalable
- Secure
- Observable
- Evolvable

These principles apply to all services, applications and platforms.

Technology choices may change.

Principles should remain stable.


# Design Philosophy

Design systems for:

- Change
- Failure
- Growth

Do not design only for current requirements.

Assume:

- Requirements will evolve
- Traffic will grow
- Integrations will increase
- Failures will occur

Good design anticipates change.


# Domain Design Principles

Systems should be organized around business domains.

Prefer:

- Clear ownership
- Clear responsibilities
- Clear boundaries

Avoid:

- Shared responsibilities
- Undefined ownership
- Cross-domain coupling

Every component should have a clearly defined purpose.


# Service Design Principles

Each service should:

- Have a single primary responsibility
- Own its business logic
- Minimize dependencies
- Expose clear interfaces

Avoid:

- God services
- Circular dependencies
- Shared mutable state


# Data Design Principles

Data ownership must be explicit.

Prefer:

- Single source of truth
- Clear ownership
- Controlled data sharing

Avoid:

- Multiple sources of truth
- Hidden dependencies
- Database coupling

Services own their data.


# Integration Principles

Integrations should be:

- Explicit
- Observable
- Versioned when necessary
- Resilient to failure

Prefer:

- Contract-based integrations
- Loose coupling
- Event-driven communication when appropriate

Avoid:

- Hidden integrations
- Tight coupling
- Direct dependency chains


# Reliability Principles

Design assuming failure.

Systems should support:

- Retries
- Timeouts
- Graceful degradation
- Recovery strategies

Failures should be expected and managed.

Reliability is a feature.


# Scalability Principles

Design for expected growth.

Scale based on evidence.

Avoid:

- Premature scaling
- Unnecessary distributed systems

Invest in scalability when justified by business needs.


# Security Principles

Security must be considered by design.

Apply:

- Least privilege
- Secure defaults
- Defense in depth
- Secrets management

Security should not be added later.


# Observability Principles

Systems must provide:

- Logs
- Metrics
- Traces
- Health checks

Failures should be detectable.

Unknown failures are unacceptable.


# Evolution Principles

Architectures should support evolution.

Prefer:

- Modular designs
- Incremental improvements
- Backward compatibility when possible

Avoid:

- Big-bang rewrites
- Unnecessary migrations

Systems should evolve continuously.


# AI Requirements

When proposing system designs:

Always evaluate:

- Domain boundaries
- Data ownership
- Failure scenarios
- Scalability needs
- Security implications
- Observability requirements
- Evolution impact

Design systems, not isolated features.