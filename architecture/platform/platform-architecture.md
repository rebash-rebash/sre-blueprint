
# Platform Architecture

## Recommended Flow

Applications
    ↓
OpenTelemetry
    ↓
Prometheus + Loki + Tempo
    ↓
Grafana
    ↓
Alertmanager
    ↓
Slack / PagerDuty

GitLab CI/CD
    ↓
ArgoCD
    ↓
Kubernetes
