## Volumes

* A Container is ephemeral, there is no state in the container
* In order to save data, it needs a disk mounted, or volume
* Network storage can be attached.
* Volumes are very common
* "k describe pod mealie..."
	* Volumes:
	~~~
	kube-api-access-m7jlw:
		Type:Projected (a volume that contains injected data from multiple sources)
		TokenExpirationSeconds:  3607
		ConfigMapName:           kube-root-ca.crt
		ConfigMapOptional:       <nil>
		DownwardAPI:             true
	~~~
* Can define an "emptyDir" first for ephemeral storage.
* Scratch Volume on a pod example:
	~~~
	spec:
		containers:
		    - image: nginx
		    name: nginx-yaml
		    volumeMounts:
			    - mountPath: /scratch
		          name: scratch-volume
		volumes:
		    - name: scratch-volume
		      emptyDir:
				sizeLimit: 500mi
	~~~
* API Spec 

Links:
[[Kubernetes Fundamentals]]


202501210503