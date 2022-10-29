Node : Worker Machine , which runs a Application
Cluster Of Nodes: Group of Nodes
Master : Which manages the nodes




Components That Are Installed on Default while installing Kubernetes:
- API Server -> Acts as FE for Kubernetes
- etcd store -> Key-Value Store used to store all data used to manage the cluster.
- Scheduler -> Responsible to distribute work or containers across multiple nodes
-  Controller -> Noticing and Responses when Some node goes down
- Container RunTime -> Docker
- Kubelet -> It is a agent runs on each node it will make sure that the containers  are working as expected.



Master
- Kube-apiserver
- etcd
- controller
- Scheduler

Worker Node:
- Kubelet
- Container Run Time


[[Kubectl]] is Used to deploy and manage applications on a kubernetes cluster.
