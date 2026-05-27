
# Payment API Runbook

## Symptoms

- Increased 5xx errors
- High latency
- Pod crashes

## Investigation

### Check pods

```bash
kubectl get pods -n payments
```

### Check logs

```bash
kubectl logs deployment/payment-api -n payments
```

### Check metrics

- Error rate
- CPU usage
- DB latency

## Rollback

```bash
helm rollback payment-api
```

## Escalation

- Payments Team
- Platform Team
