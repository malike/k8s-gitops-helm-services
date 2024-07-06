### Helm Packaging for Services


Helm charts for both frontend and backend services.


## Helm Chart Repository

It also serves as a helm repository, where you helm releases for both services.

### Usage
Helm must be installed to use the charts.

```shell
helm repo add gitops-observability https://malike.github.io/k8s-gitops-helm-services/
```

This is a  one time activity.

To install the frontend.

```shell
helm install gitops-frontend gitops-observability/gitops-observability-frontend-chart
```

To install the backend.

```shell
helm install gitops-backend gitops-observability/gitops-observability-backend-chart
```


To uninstall the chart:

```shell
helm delete {chart-name}
```