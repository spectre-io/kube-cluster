# Kube Cluster

GitOps-managed Kubernetes cluster configuration using Flux CD.

## Structure

- **apps/** - Application deployments (base & staging overlays)
- **clusters/** - Cluster-specific Flux configurations  
- **infrastructure/** - Infrastructure controllers (ingress, cert-manager, etc.)
- **monitoring/** - Monitoring stack configs and controllers

## Quick Start

1. Bootstrap Flux: `flux bootstrap github --owner=<user> --repository=kube-cluster`
2. Applications sync automatically from `apps/` and `infrastructure/`

## Tools

- [Flux CD](https://fluxcd.io) - GitOps operator
- [Renovate](https://renovatebot.com) - Automated dependency updates
