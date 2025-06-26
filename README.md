# homelab-platform

## 🚀 Deployment Steps

1. ./bootstrap.sh                       # Install ArgoCD
2. kubectl apply -f argocd-applications.yaml  # Deploy 3 main apps
3. Watch ArgoCD deploy everything via public Helm charts

## 🌐 Services (via Istio Gateways)

- ArgoCD:    http://argocd.dev.cluster.local
- Vault:     http://vault.dev.cluster.local  
- Keycloak:  http://keycloak.dev.cluster.local
- Kibana:    http://kibana.dev.cluster.local

## ✅ Uses Public Helm Charts

- istio-release.storage.googleapis.com/charts
- helm.releases.hashicorp.com (Vault)
- charts.bitnami.com/bitnami (Keycloak)  
- helm.elastic.co (ECK Operator)
- kyverno.github.io/kyverno (Kyverno)
