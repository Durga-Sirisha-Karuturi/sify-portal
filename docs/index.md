# Sify Developer Portal

Welcome to the **Sify Developer Portal** — internal platform for managing services, Kubernetes clusters, and APIs.

## Overview

This portal provides:

- **Service Catalog** — all registered services across the organization
- **Kubernetes** — live pod and cluster status
- **APIs** — all registered APIs
- **Metrics Dashboard** — real-time infrastructure overview

## Quick Links

- [Live App](http://10.0.1.20:30080)
- [Kubernetes Cluster](http://10.0.1.20:3000/catalog/default/component/sify-portal/kubernetes)

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | HTML, CSS, JavaScript |
| Server | Nginx (Alpine) |
| Container | Docker |
| Orchestration | Kubernetes (RKE2) |
| Portal | Backstage |
