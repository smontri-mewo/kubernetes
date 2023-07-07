# Install prometheus

helm repo add prometheus-community https://prometheus-community.github.io/helm-charts

helm repo add stable https://charts.helm.sh/stable

helm repo update

kubectl port-forward deployment/prometheus-grafana 3000