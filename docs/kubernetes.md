# Kubernetes Setup

## Cluster Info

- **Cluster**: zabbix-cluster
- **Namespace**: default
- **Replicas**: 2

## Resources

```yaml
resources:
  requests:
    memory: "64Mi"
    cpu: "50m"
  limits:
    memory: "128Mi"
    cpu: "100m"
```

## Service

- **Type**: NodePort
- **Port**: 80
- **NodePort**: 30080

## Backstage Integration

Service account `backstage-admin` has cluster-admin access for monitoring pods, logs, and deployments.
