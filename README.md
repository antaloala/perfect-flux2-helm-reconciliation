# Perfect flux2 Helm-release reconciliation

## Scope
Use flux2 kustomization (wrapping a flux2 HelmRelease) and k8s kustomize's configmapGenerators to have a perfect periodic GitOps based Helm release reconciliation.

## Use Cases
1. To recreate a manually Helm uninstalled (Helm) release.

2. to recreate (from a periodically reconciled Helm release) those API objects owned by a Helm release when being manually deleted through some `kubectl delete` command.
