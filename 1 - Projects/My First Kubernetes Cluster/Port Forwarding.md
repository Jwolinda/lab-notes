
You can forward one or more local ports to a pod. 
```
kubectl port-forward pod/mypod 5000 6000
```

This allows me to avoid using a service when testing a single pod.

Links:

[[Kubernetes Fundamentals]]
[[Networking]]

202501201444