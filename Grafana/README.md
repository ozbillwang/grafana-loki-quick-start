# https://grafana.com/docs/loki/latest/setup/install/helm/install-monolithic/

Good practices to set values.yaml files for different environments

```
kubens loki

helm upgrade --install --namespace=loki --values values-staging.yaml loki-grafana grafana/grafana
```
