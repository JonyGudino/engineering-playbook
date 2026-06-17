<!-- 
1. Purpose

2. Observability Philosophy

3. Telemetry Principles

4. Logging Standards

5. Metrics Standards

6. Tracing Standards

7. Health Monitoring

8. Alerting Principles

9. Incident Investigation

10. Operational Visibility

11. Business Observability

12. AI Requirements
 -->

# Purpose

The purpose of these standards is to ensure systems provide sufficient visibility to understand, operate and improve production environments.

Observability should enable teams to:

- Detect issues
- Investigate failures
- Measure system health
- Understand user impact
- Support continuous improvement

Observability is required for reliable operations.


# Observability Philosophy

Systems should be observable by design.

Observability should answer:

- What happened?
- Why did it happen?
- Who was affected?
- Is the issue ongoing?

Observability should reduce uncertainty during operations and incident response.

Unknown system behavior is unacceptable.


# Telemetry Principles

Systems should emit telemetry that reflects their behavior.

Telemetry may include:

- Logs
- Metrics
- Traces
- Events

Telemetry should be:

- Consistent
- Actionable
- Correlated
- Accessible

Telemetry should support operational decision-making.


# Logging Standards

Logs should provide meaningful operational context.

Logs should:

- Be structured when possible
- Include relevant identifiers
- Support troubleshooting
- Avoid sensitive information exposure

Avoid:

- Excessive logging
- Ambiguous messages
- Logging secrets

Logs should help explain system behavior.


# Metrics Standards

Metrics should measure system behavior over time.

Metrics should focus on:

- Availability
- Reliability
- Performance
- Capacity
- Business outcomes when appropriate

Metrics should support trend analysis and operational decisions.


# Tracing Standards

Distributed workflows should be traceable.

Tracing should support:

- Request tracking
- Dependency analysis
- Latency investigation
- Failure analysis

Traceability should extend across system boundaries whenever possible.


# Health Monitoring

Systems should expose their operational health.

Health monitoring should provide visibility into:

- Availability
- Dependencies
- Resource utilization
- Service readiness

Health information should support automated and manual operations.


# Alerting Principles

Alerts should indicate actionable conditions.

Alerts should be:

- Relevant
- Actionable
- Prioritized

Avoid:

- Alert fatigue
- Excessive noise
- Non-actionable alerts

Every alert should have a defined response path.


# Incident Investigation

Systems should support efficient incident investigation.

Operational data should enable:

- Root cause analysis
- Timeline reconstruction
- Impact assessment
- Recovery validation

Incident investigation should rely on evidence, not assumptions.


# Operational Visibility

Operational teams should have visibility into:

- Service health
- Dependency health
- System performance
- Error conditions
- Capacity trends

Operational visibility should support proactive management.


# Business Observability

Observability should extend beyond technical metrics.

Measure:

- User impact
- Critical workflows
- Business events
- Service adoption

Business observability connects technical performance with business outcomes.


# AI Requirements

When proposing solutions, always evaluate:

- Logging requirements
- Metrics requirements
- Tracing requirements
- Health monitoring needs
- Alerting implications
- Operational visibility needs
- Business observability opportunities

Identify observability gaps.

Recommend telemetry improvements.

Recommend ADR creation when observability decisions have long-term impact.