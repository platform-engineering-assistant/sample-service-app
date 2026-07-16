# Sample Service App

This repository represents a small service owned by an application developer.
The developer owns the container definition and the platform deployment
configuration.

The app container is defined in `app/Dockerfile`. Kubernetes deployment is
managed through Helm and Argo CD:

- `charts/sample-service-app/` contains the Helm chart.
- `argocd/sample-service-app.yaml` contains the Argo CD `Application`.

## Render Manifests

```sh
helm template sample-service-app charts/sample-service-app
```

## Deploy With Argo CD

Apply the Argo CD application manifest to a cluster with Argo CD installed:

```sh
kubectl apply -f argocd/sample-service-app.yaml
```
