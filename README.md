Pre-Install: 
* kuberntes cluster;
* helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
* helm repo update
* kubectl create ns monitoring
* helm install -n monitoring prometheus-operator prometheus-community/kube-prometheus-stack


