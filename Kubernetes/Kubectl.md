- Kubectl run 
- kubectl cluster-info
- kubectl get nodes


the convention is to use kubectl apply to create AND update resources, kubectl create is used to create resources, and kubectl run is used to create a pod with a specific image, namespace, etc. for experimentation and testing with the --dry-run=client option.



- create
		- kubectl create
- Get
		- kubectl get
		- kubectl get -o wide
		- kubectl describe
- Update
		- kubectl apply (file)
		- kubectl set (value)
- status
		- kubectl rollout status
		- kubectl rollout history
- rollback 
		- kubectl rollout undo 
