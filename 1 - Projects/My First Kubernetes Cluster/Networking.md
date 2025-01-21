* There are not infinite IP Addresses
* Freeing up IPs can be useful
* By Default all pods can connect to any other pod on the network.
	* Network Policies control this
	* i.e. restrict to anything not in its namespace
* Pods are kind of like lightweight VMs
	* Containers on a pod can talk to each other on localhost
* Container Networking Interface plugin
	* Each container has a networking interface
	* This sets up routes and IP Addresses
	* Iptables is configured for each node
	* Some popular ones:
		* Cilium
		* Calico
		* Flannel
* "rdctl" - Rancher Desktop CTL
* Avoid Node Ports
* Load Balancer is used with cloud often.
* 

## Services

* A service offers a consistent address to access a set of pods
* Why do we need services?
	* Pods are ephemeral
	* Pods are constantly updating  and you cannot expect a pod to continue to be around.
	* A service is basically a grouping of pods
* A frontend service can be attached to a group of pods and then we don't have to worry about which pod gets which request.
* Would normally do from code, but can use command line "expose" command
* "k expose deployment test-deployment --port 8080"

## Ingress

* Advanced topic
	* Should do an overview
* Allows for a FQDN
* Mischa does it via Cloudflare tunnels
* Exposes http/https routes from outside the cluster into the cluster
* SSL & TLS Termination
* External URL
* Path Based Routing
* Ingress Controller
	* NBINX
	* Traefik
	* Cilium
	* AGIC
* We have Traefik in Rancher Desktop
* Ingress -> Routing Rule -> Service -> Po


Links:

[[Kubernetes Fundamentals]]
[[Rancher Setup for Windows and WSL2]]

202501201525