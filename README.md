# Kubernetes GitOps

Declarative Kubernetes deployment configuration for the food platform.

## Planned scope

- Frontend and backend workloads
- Services, ingress, and autoscaling
- Environment overlays
- GitOps controller applications and policies

## Repository conventions

- Base manifests or charts are separated from environment overlays.
- Every change is reviewed and reconciled through GitOps.
- Container image tags are immutable.
- Plain-text secrets must never be committed; use the approved secret-management solution.

Cluster provisioning belongs in `terraform-infrastructure`.
