
# Pod CrashLoop Runbook

## Investigation Steps

```bash
kubectl describe pod <pod-name>
```

```bash
kubectl logs <pod-name>
```

## Common Causes

- Bad image
- Missing secret
- Resource limits
- Database connectivity

## Resolution

- Rollback deployment
- Fix configuration
- Increase resources
