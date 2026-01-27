# Helm Guestbook with Multiple Sources

This example demonstrates ArgoCD's **multiple sources** feature, where a single Application uses two sources:

1. **Chart source** (`chart/` directory) - Contains the Helm chart with templates and default values
2. **Values source** (`values/` directory) - Contains custom values that override the chart defaults

## Directory Structure

```
helm-guestbook-multiple-sources/
├── chart/                    # First source: The Helm chart
│   ├── Chart.yaml
│   ├── values.yaml          # Default values
│   └── templates/
│       ├── _helpers.tpl
│       ├── NOTES.txt
│       ├── deployment.yaml
│       └── service.yaml
├── values/                   # Second source: Custom values
│   └── custom-values.yaml   # Overrides for chart values
├── application.yaml          # ArgoCD Application manifest
└── README.md
```

## How It Works

The Application manifest (`application.yaml`) uses the `sources` field (plural) instead of `source` (singular):

- **Source 1**: Points to the `chart/` directory and references values from the second source using `$values` variable
- **Source 2**: Points to the repository root with `ref: values`, making it available as `$values` for the Helm chart

This pattern is useful when:
- You want to use an external/public Helm chart with your own custom values
- You want to separate chart management from environment-specific values
- You need to override values without modifying the original chart

## Deployment

To deploy this application to ArgoCD:

```bash
kubectl apply -f application.yaml
```

Or using the ArgoCD CLI:

```bash
argocd app create -f application.yaml
```

## Key Configuration

In the `application.yaml`, note the multiple sources configuration:

```yaml
sources:
  - repoURL: https://github.com/argoproj/argocd-example-apps.git
    path: helm-guestbook-multiple-sources/chart
    targetRevision: HEAD
    helm:
      valueFiles:
        - $values/helm-guestbook-multiple-sources/values/custom-values.yaml
  - repoURL: https://github.com/argoproj/argocd-example-apps.git
    targetRevision: HEAD
    ref: values
```

The `ref: values` in the second source maps to the `$values` variable used in the first source's `valueFiles`.

## Customization

To customize the deployment, edit `values/custom-values.yaml`. The values there will override the defaults in `chart/values.yaml`.

Current customizations:
- `replicaCount`: 3 (vs default 5)
- `service.type`: LoadBalancer (vs default ClusterIP)
- `resources`: Defined limits and requests (vs default empty)
- `image.pullPolicy`: Always (vs default IfNotPresent)

## Reference

For more information about ArgoCD's multiple sources feature, see:
https://argo-cd.readthedocs.io/en/latest/user-guide/multiple_sources/
