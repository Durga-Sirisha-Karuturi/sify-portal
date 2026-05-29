# Deployment Guide

## Prerequisites

- Docker installed
- Kubernetes cluster access
- kubectl configured

## Steps

### 1. Build Docker Image

```bash
cd ~/sify-portal
docker build -t sify-portal:latest .
```

### 2. Deploy to Kubernetes

```bash
kubectl apply -f k8s/deployment.yaml
```

### 3. Verify

```bash
kubectl get pods -l app=sify-portal
kubectl get svc sify-portal
```

### 4. Access

Open browser: `http://10.0.1.20:30080`

## Update Deployment

```bash
docker build -t sify-portal:latest .
kubectl rollout restart deployment/sify-portal
```
