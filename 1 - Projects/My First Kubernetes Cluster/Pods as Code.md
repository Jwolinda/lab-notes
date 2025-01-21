* Pods are defined in YAML.
* You can edit on the cluster, and will need to know how to for the [[KCTA Exam]], but that is not how you'll actually use them in dev/prod. 
* Dry Run
	* You can use dry run to print  the corresponding API objects without creating them.
	* Client will only export the output on the client
	* Server will submit the resource without persisting
* Applying Files to our cluster
	* Create
		* This method only creates it 
	* Apply
		* This method applies and does both
		* -f, --filename
			* Applies based on a file passed as an argument.
			* Looks like we can apply either JSON or YAML?
* You can get at YAML examples quickly in the docs by searching for "Version"
* [[vim]] trick: Use command ":set paste" to preserve formatting when copying and pasting from the docs


Links:
[[Pods]]
[[Kubernetes Fundamentals]]
202501200834