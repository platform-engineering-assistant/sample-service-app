# Sample Service App

This repository represents a small service owned by an application developer.
The developer owns the container definition but has not written Kubernetes,
Helm, or Argo CD configuration.

The platform assistant can inspect `app/Dockerfile` and prepare the deployment
configuration from platform standards and policies:

```text
Deploy sample-service-app
```

The initial repository deliberately contains no `charts/` or `argocd/`
directory. Generated files are written locally only after explicit approval.
