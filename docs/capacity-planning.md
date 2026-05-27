# Capacity Planning

## Purpose

Capacity planning ensures services have the resources needed to meet demand without overprovisioning.

## Key Concepts

- Baseline utilization
- Forecasting demand
- Headroom and buffer
- Scaling policy
- Review cadence

## Process

1. Inventory all services, infrastructure, and resource types.
2. Collect historical usage for CPU, memory, disk, network, and request throughput.
3. Define expected growth rates and seasonality.
4. Identify the capacity threshold for each environment.
5. Plan buffer and safety margins for peak traffic and incident recovery.
6. Review capacity plans monthly or before major releases.

## Deliverables

- Capacity model for each environment
- Capacity runbook for scaling actions
- Budget and cost estimates for growth
- Risk assessment for hotspots

## Best Practices

- Use objective metrics, not guesses
- Tie capacity planning to SLOs and error budgets
- Keep emergency scale-up playbooks accessible
- Automate capacity alerts where possible
