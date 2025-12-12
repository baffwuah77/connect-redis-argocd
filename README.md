# Connect-Redis ArgoCD

Redis deployment managed by ArgoCD.

## Structure
```
connect-redis-argocd/
├── argocd-app.yaml          # ArgoCD Application definition
├── manifests/               # Kubernetes manifests
│   ├── namespace.yaml
│   ├── deployment.yaml
│   └── service.yaml
├── base/                    # Kustomize base
│   └── kustomization.yaml
└── overlays/                # Environment overlays
    ├── dev/
    ├── staging/
    └── prod/
```

## Deploy to ArgoCD
```bash
kubectl apply -f argocd-app.yaml
```

## Repository

https://github.com/baffwuah77/connect-redis-argocd
