# Docker-Kubernetes


## Deploying microservices
The microservices is a simple app containing:

 - Front end application(Python)
 
 Build the image using Dockerfile in vote directory
 
 - Back end application(Node.js)
 
 Build the mages using Dockerfile in result directory
 
 - Redis
 
 For messaging
 
 - Postgres
 
 For storage
 
 - Worker app(.NET)
 
 Build the image using Dockerfile in Worker directory
 
 ## Monitoring( Prometheus, grafana ) using helm
 
 - Install Helm
 - helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
 - helm repo add stable https://charts.helm.sh/stable
 - helm repo update
 - helm install prometheus prometheus-community/kube-prometheus-stack
 - kubectl port-forward deployment/prometheus-grafana 3000 ( enabling port forward inorder to access Grafana )
 
