# kubernetes-commands
(Hobby) Here are some very common CLI commands used when working with kubernetes 

Here is the hierarchy when using Kubernetes:  
Cluster > Node > Pod > Container > App / Server / DB  

```
kubectl get svc  # kubectl get service  
kubectl get svc -n develop1  # get the service with name develop1
kubectl get ns  # kubectl get namespace 
kubectl get pod  #  
kubectl get  
kubectl get  
kubectl get  
kubectl get  
kubectl get  

# Create Namespaces  
kubectl create ns develop1  

# Deploy all K8s objects from develop1  
kubectl get all -n develop1
```
