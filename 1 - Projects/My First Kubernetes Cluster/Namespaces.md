* "k get namespaces"
* Namespaces are a mechanism for isolating groups of resources within a single cluster
	* Applicable on namespaced objects (Deployments, Services, etc.)
	* Not Applicable on cluster wide objects (StorageClass, Nodes, PersistentVolumes, etc.)
* Namespaces should be based on Projects/Applications, possibly team based.
	* Airflow
	* Encompass
* Access Control can be on the namespace level
* -n is shorthand for --namespace
* setting my namespace to a new one - **[[IMPORTANT]]**
	* **"k config set-context --current --namespace=mealie "**


Links:
[[Kubernetes]]
[[Kubernetes Fundamentals]]

202501201407