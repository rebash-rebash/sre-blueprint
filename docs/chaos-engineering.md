# Chaos Engineering

## Purpose

Chaos engineering helps teams verify resilience by intentionally testing failure modes in a controlled manner.

## Principles

- Start with a hypothesis
- Use small, safe experiments
- Observe how systems behave under failure
- Learn and improve continuously

## Experiment Workflow

1. Define the reliability hypothesis.
2. Select a targeted failure mode.
3. Establish guardrails and blast radius.
4. Execute the experiment.
5. Collect observations.
6. Review results and update remediation.

## Common Experiments

- Pod or node termination
- Service latency injection
- Dependency failure simulation
- Resource exhaustion

## Safety Controls

- Run experiments in non-production first
- Use feature flags and circuit breakers
- Monitor SLOs and alerting during experiments
- Roll back quickly if needed

## Output

- Document experiment objective
- Capture observed behavior
- Define follow-up actions
- Update incident and resiliency runbooks
