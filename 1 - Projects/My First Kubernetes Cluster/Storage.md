
### Ephemeral Volumes
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
* Able to update files across containers on a single pod.


### Persistent Volumes

* Two types:
	* Persistent Volumes
		* Like a huge disk
		* One app will request a small part of the disk
	* Persistent Volume Claims
		* Claiming a piece of the disk
		* They can be configured in YAML or dynamically
		* This is the most common use case
		~~~
		 apiVersion: v1
		    kind: PersistentVolumeClaim
			metadata:
			    name: mealie-data
			    namespace: mealie
			spec:
			    accessModes:
				    - ReadWriteOnce
		    resources:
			    requests:
				    storage: 500Mi   
		~~~

	* Use in a deployment:
	```
     spec:
      containers:
        - image: ghcr.io/mealie-recipes/mealie:v1.3.2
          name: mealie
          ports:
            - containerPort: 9000
          volumeMounts:
            - mountPath: /app/data
              name: mealie-data
      volumes:
        - name: mealie-data
          persistentVolumeClaim:
            claimName: mealie-data
	```

Links:
[[Kubernetes Fundamentals]]


202501210503