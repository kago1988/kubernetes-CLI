# kubernetes-CLI
(Hobby) Here are some very common CLI commands used when working with kubernetes 

Here is the hierarchy when using Kubernetes:  
Cluster > Node > Pod > Container > App / Server / DB  

```
flags often used:  
-f = force  
-n = name  
-ns = namespace  

kubectl get svc  # list services  
kubectl get svc -n develop1  # list the service from name develop1
kubectl get ns  # list the namespaces  
kubectl get nodes  # list the nodes  
kubectl get pods  # list the pods  
kubectl get pods -n develop1  # list the pods from name develop1 
kubectl get deploy -n develop1  # get deploy from name develop1  
kubectl get quota -n develop1  # get quota from name develop1  
kubectl get  
kubectl get  


kubectl create ns develop1 # Create Namespace  
kubectl delete ns develop1 # Delete Namespace  
kubectl get all -n develop1 # List all objects from namespace develop1  
kubectl apply -f kube-manifest # Deploy all K8s objects from develop1  


kubectl get limits -n develop1  # get limits  
kubectl describe limits default-cpu-mem-limit-range -n develop1  # describe limits  
```
