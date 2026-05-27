
# Loki Setup

## Install Loki Stack

```bash
helm repo add grafana https://grafana.github.io/helm-charts

helm install loki grafana/loki-stack       -n monitoring
```
