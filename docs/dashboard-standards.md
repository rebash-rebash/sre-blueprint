# Dashboard Standards

## Purpose

Dashboards should provide fast insight into service health, reliability, and operational status.

## Dashboard Sections

- Service health summary
- SLO / error budget status
- Key performance metrics
- Dependency and infrastructure view
- Alert and incident status

## Design Guidelines

- Keep dashboards focused and easy to read
- Use consistent naming and layout across services
- Annotate significant events or deployment changes
- Provide links to related runbooks and incidents

## Recommended Panels

- Request rate and success rate
- Latency percentiles
- Error budget burn rate
- Resource utilization (CPU, memory)
- External dependency health

## Metadata

- Owner team
- Service name
- Update frequency
- Related runbook link

## Best Practices

- Build one overview dashboard per service
- Use dedicated dashboards for SRE and on-call views
- Avoid duplicate dashboards with the same metrics
- Keep dashboard definitions under source control
