# Install prometheus

helm repo add prometheus-community https://prometheus-community.github.io/helm-charts

helm repo add stable https://charts.helm.sh/stable

helm repo update

helm install stable prometheus-community/kube-prometheus-stack -n monitoring

kubectl port-forward deployment/stable-grafana 3000

User: admin
Pwd: prom-operator

Dashboard	ID
k8s-addons-prometheus.json	19105
k8s-addons-trivy-operator.json	16337
k8s-system-api-server.json	15761
k8s-system-coredns.json	15762
k8s-views-global.json	15757
k8s-views-namespaces.json	15758
k8s-views-nodes.json	15759
k8s-views-pods.json	15760
