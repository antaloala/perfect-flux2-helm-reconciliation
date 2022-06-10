# Perfect flux2 Helm-release reconciliation

## Scope
Use flux2 kustomization (wrapping a flux2 HelmRelease) and k8s kustomize's configmapGenerators to have a perfect automatic periodic GitOps based reconciliation on a Helm release.

## Use Cases
1. To automatically recreate a manually Helm uninstalled (Helm) release.

2. to automatically recreate (from a periodically reconciled Helm release) those API objects owned by a Helm release that have been  manually deleted through some `kubectl delete` command.
