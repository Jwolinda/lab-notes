
## Rancher UI Overview

* Can see and manage your running containers
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
* An init container does just one task and then stops running
* Some configuration types available are:
	* Single Container
	* Multi Container
	* Init Container
	* Networking
	* Storage
* Storage lets all the different pods use the same storage (Important)
* [[Pods as Code]] are written in YAML
* 

## Control Plane

* Scheduler controls which worker node gets the pod.
* API Server accepts requests and routes to other controller node processes.

## Interacting w/ Pods

* Deleting Pods
	* "k delete pod..."
	* Can be deleted based on filename with -f
	* Can be deleted based on label -l
	* Can be just deleted based on name
* Interacting with the pod directly
	* "k exec -it nginx -- /bin/bash"
		* -i = Pass stdin to the container (from my terminal)
		* -t = STDIN is a [[TTY]]
			* https://www.linusakesson.net/programming/tty/index.php
	* Only works because we've hooked up the i and t flags
	* We were logged into the only container running in that pod
	* you must use two dashes (--) to separate your command's flags/arguments 
	> This is essential for prod and will get you one step ahead of the pack
	
	
* Security
	* "curl {podIp}"
	* It's important to have strict security measures in place.
	* If someone can get access to a container running on one of your pods, we need to make sure they cannot network with the other pods in a way that circumvents how we want information to flow.

Links:

[[Kubernetes Fundamentals]]


202501191748