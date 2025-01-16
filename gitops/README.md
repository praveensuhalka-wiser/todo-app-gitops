# Todo App GitOps Configuration

This repository contains the Kubernetes manifests and Argo CD configurations for the Todo application deployment.

## Structure

```
.
├── apps/
│   ├── base/                 # Base configurations
│   └── overlays/            # Environment-specific overlays
│       ├── dev/
│       ├── staging/
│       └── prod/
├── bootstrap/               # Argo CD bootstrap configurations
└── applicationset/          # ApplicationSet configurations
```

## Prerequisites

- Kubernetes cluster
- Argo CD installed
- Helm (for managing some dependencies)

## Usage

1. Install Argo CD in your cluster
2. Apply the ApplicationSet configuration
3. Argo CD will automatically sync the applications
