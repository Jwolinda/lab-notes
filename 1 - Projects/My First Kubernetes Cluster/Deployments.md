
* You don't really run single pods with Kubernetes.
* Applications with multiple instances need deployment.
## How to Orchestrate

* "k create deployment"
	* This is where you can tell the deployment that you need replicas
	* Deployments are a way of communicating a desired state to Kubernetes.
* deployments : pods - 1 : *
* Autocomplete bringing up "deployments.apps" is an artifact of the API naming convention
* Can be edited: "k edit deployment ..."
* You can use dry run in this environment as well.

## Replica Sets

* Replica sets describe the desired replicas in a deployment
* Replicas should not truly be managed by users
	* They are managed by deployments
	* Old Replica Sets are kept so we can roll back
		* Default of 10
* Rolling Update by default
* Can update

	```
	spec:
		strategy:
			type: RollingUpdate
			rollingUpdate:
		      maxUnavailable: 1 -- Also can be %
		      maxSurge: 1
	```

* watch -n 1 "kubectl get pods" 
* Can deployments have different kinds of containers?
* Recreate Strategy gets rid of all at once
* Gave developed a bug to showcase rollout with the following:
	```
    spec:
      containers:
        - image: httpd:alpine3.18
          name: httpd
          command: ["/bin/bash", "c"]
          args: ["sleep 5; exit 1"]
	```

Links:
[[Pods]]
[[Pods as Code]]
[[Kubernetes Fundamentals]]
202501201016