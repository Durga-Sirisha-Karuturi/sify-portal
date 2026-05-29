# Architecture

## Overview

This project hosts a static web portal (`sify-portal`) deployed on Kubernetes and served through Nginx.

### Request Flow

```text
Browser
   │
   ▼
NodePort Service (30080)
   │
   ▼
Kubernetes Service
   │
   ▼
sify-portal Deployment (2 Replicas)
   │
   ▼
Nginx Pods
   │
   ▼
Static HTML/CSS/JavaScript Content
