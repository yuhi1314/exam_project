Pre-Install: 
* kuberntes cluster;




For adding monitoring:
* helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
* helm repo update
* helm install -n monitoring prometheus-operator prometheus-community/kube-prometheus-stack


