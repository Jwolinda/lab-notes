
## A Story

* Using all of these VMs
	* Each one might contain a couple applications
* Containerization came along in mainstream 2013
	* Allows us to have multiple containers on one machine
* Moved towards a couple VMs with a bunch of docker containers on them.
	* All of these use a CPU and share a pool of compute.
	* What if we want replicas of our applications?
		* Front ends
	* End up with a super elaborate system with ansible playbooks
	* These containers don't have context that the others are there
	* Have to use HA PROXY load balancers
* Kubernetes is the same, but there is a controller node and worker nodes
* Desired outcomes are placed in a YAML file
* Worker Nodes and replication can be scaled pre-emptively or JIT for demand matching.

>  Kubernetes is the operating system of the cloud

\- Mischa Van Den Berg, 2024



Links:

[[Kubernetes Fundamentals]]


202501191548