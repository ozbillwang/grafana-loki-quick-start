# https://grafana.com/docs/loki/latest/setup/install/helm/install-monolithic/

Good practices to set values.yaml files for different environments

```
helm repo add grafana https://grafana.github.io/helm-charts

helm repo update

kubectl create ns loki
kubens loki

helm -n loki upgrade --install --values values-staging.yaml loki grafana/loki

