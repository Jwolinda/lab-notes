
* Monitoring stack
* Able to install using helm kube-prometheus-stack
```
helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
helm repo update
```
* Grafana allows for visualizations
~~~
helm show values prometheus-community/kube-prometheus-stack > secrets 
~~~
* Able to use this to get configurations 


Links
[[Kubernetes Fundamentals]]

202501211902