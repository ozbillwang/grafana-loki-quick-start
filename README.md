# Grafana Loki Guick Start

Reference: https://grafana.com/docs/loki/latest/setup/install/helm/install-monolithic/

```
helm repo add grafana https://grafana.github.io/helm-charts

helm repo update

kubectl create ns loki
kubens loki

# depends on AWS or Azure

# AWS
helm -n loki upgrade --install --values values-aws.yaml loki grafana/loki

# Azure
helm -n loki upgrade --install --values values-azure.yaml loki grafana/loki
```
