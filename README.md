Pre-Install: 
Kubernetes
Install Prometheus Operator inside monitoring namespace.

Install helm.

brew install helm
Add prometheus-community repo and update helm.

helm repo add prometheus-community https://prometheus-community.github.io/helm-charts

helm repo update
Create monitoring namespace inside kubernetes.

kubectl create ns monitoring
Install operator.

helm install -n monitoring prometheus-operator prometheus-community/kube-prometheus-stack --set prometheus-node-exporter.hostRootFsMount=false

