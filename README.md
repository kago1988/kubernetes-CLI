# kubernetes-CLI
(Hobby) Here are some very common CLI commands used when working with kubernetes 

Here is the hierarchy when using Kubernetes:  
Cluster > Node > Pod > Container > App / Server / DB  

```
flags often used:  
-f = force  
-n = name  
-o = output format  

kubectl get svc  # list services  
kubectl get svc -n develop1  # list the service from name develop1
kubectl get ns  # list the namespaces  
kubectl get nodes  # list the nodes  
kubectl get pods  # list the pods  
kubectl get pods -n develop1  # list the pods from name develop1 
kubectl get deploy -n develop1  # get deploy from name develop1  
kubectl get quota -n develop1  # get quota from name develop1  
kubectl get nodes -o wide  # list nodes with a lot of details   
kubectl get sc  # list storage classes  


kubectl create ns develop1 # Create Namespace  
kubectl delete ns develop1 # Delete Namespace  
kubectl get all -n develop1 # List all objects from namespace develop1  
kubectl apply -f kube-manifest # Deploy all K8s objects from develop1  
kubectl delete -f kube-manifest/  # Delete the kube-manifest  


kubectl get limits -n develop1  # get limits  
kubectl describe limits default-cpu-mem-limit-range -n develop1  # describe limits  
```

Less frequently used are: 
```
kubectl annotate - Update the annotations on a resource 
kubectl api-resources - Print the supported API resources on the server  
kubectl api-versions - Print the supported API versions on the server, in the form of "group/version"  
kubectl apply - Apply a configuration to a resource by filename or stdin  
kubectl attach - Attach to a running container  
kubectl auth - Inspect authorization  
kubectl autoscale - Auto-scale a Deployment, ReplicaSet, or ReplicationController  
kubectl certificate - Modify certificate resources.  
kubectl cluster-info - Display cluster info  
kubectl completion - Output shell completion code for the specified shell (bash or zsh)  
kubectl config - Modify kubeconfig files  
kubectl cordon - Mark node as unschedulable  
kubectl cp - Copy files and directories to and from containers.  
kubectl create - Create a resource from a file or from stdin.  
kubectl debug - Create debugging sessions for troubleshooting workloads and nodes  
kubectl delete - Delete resources by filenames, stdin, resources and names, or by resources and label selector  
kubectl describe - Show details of a specific resource or group of resources  
kubectl diff - Diff live version against would-be applied version  
kubectl drain - Drain node in preparation for maintenance  
kubectl edit - Edit a resource on the server  
kubectl exec - Execute a command in a container  
kubectl explain - Documentation of resources  
kubectl expose - Take a replication controller, service, deployment or pod and expose it as a new Kubernetes Service  
kubectl get - Display one or many resources  
kubectl kustomize - Build a kustomization target from a directory or a remote url.  
kubectl label - Update the labels on a resource  
kubectl logs - Print the logs for a container in a pod  
kubectl options - Print the list of flags inherited by all commands  
kubectl patch - Update field(s) of a resource  
kubectl plugin - Provides utilities for interacting with plugins.  
kubectl port-forward - Forward one or more local ports to a pod  
kubectl proxy - Run a proxy to the Kubernetes API server  
kubectl replace - Replace a resource by filename or stdin  
kubectl rollout - Manage the rollout of a resource  
kubectl run - Run a particular image on the cluster  
kubectl scale - Set a new size for a Deployment, ReplicaSet or Replication Controller  
kubectl set - Set specific features on objects  
kubectl taint - Update the taints on one or more nodes  
kubectl top - Display Resource (CPU/Memory/Storage) usage.  
kubectl uncordon - Mark node as schedulable  
kubectl version - Print the client and server version information  
kubectl wait - Experimental: Wait for a specific condition on one or many resources.  
```
See [kubernetes.io](https://kubernetes.io/docs/reference/kubectl/_print/)
