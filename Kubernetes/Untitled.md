Services Types:
	NodePort(30000-32767)
	ClusterIP
	LoadBalancer

types of namespaces:
	kube-system
	Default
	Kube-Public
DNS:
	servicename.namespace.service.domain
Pod-run
service-expose
deployment-create
con
secrets
configmap



kubectl explain pods --recursive | less
kubectl explain pods --recurisve | grep -A8 envForm