
## Rancher UI Overview

* Can see and manage your running ocntainers
* Can see images on system
* Can reset Kubernetes in UI and can reset cluster.

## KubeCTL

* You can use the documentation during the exams
* https://kubernetes.io/docs/reference/kubectl/quick-reference/
* kubectl runs on context. It is just a client to interact with the APIs that make up a Kubernetes cluster.
* kubectl explain * will bring up documentation I can pipe into a text editor to read

## Pods

* Pods are the smallest units in Kubernetes
* They exist inside of Nodes
* You cannot get to them directly, they require a [[Deployment]]
* These are a collection of containers - 1:*
* The name comes from a "pod" of whales.

## Control Plane

* Scheduler controls which worker node gets the pod.
* API Server accepts requests and routes to other controller node processes.


Links:

[[Kubernetes Fundamentals]]


202501191748