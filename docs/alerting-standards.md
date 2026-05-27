# Alerting Standards

## Purpose

Alerting standards reduce noise and ensure the right teams respond to the right events.

## Alert Categories

- Page alerts: urgent, actionable issues
- Ticket alerts: medium priority, investigation required
- Info alerts: operational insights, no immediate action

## Severity Mapping

- critical / P1: service outage or customer impact
- major / P2: major degradation
- minor / P3: localized or non-critical issue
- info / P4: informational and monitoring-only

## Rule Design Guidelines

- Alert on symptoms, not root cause
- Use stable, service-level metrics
- Require sustained conditions before firing
- Avoid overly broad selectors

## Labels and Metadata

- `severity`
- `team`
- `service`
- `runbook`

## Example

```yaml
groups:
  - name: application-alerts
    rules:
      - alert: HighErrorRate
        expr: rate(http_requests_total{status=~"5.."}[5m]) > 0.05
        for: 5m
        labels:
          severity: critical
          service: payment-api
          team: payments-team
          runbook: /runbooks/kubernetes/pod-crashloop.md
        annotations:
          summary: High error rate detected for payment-api
          description: Error rate exceeded 5% for 5 minutes
```

## Best Practices

- Track alert volume and tune thresholds
- Use service owner labels for routing
- Link alerts to runbooks and incident docs
- Review alerts periodically after incidents
