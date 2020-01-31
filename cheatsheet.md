
## kubectl trouble shooting
kubectl get - list resources 

kubectl describe - show detailed information about a resource 

kubectl logs - print the logs from a container in a pod 

kubectl exec - execute a command on a container in a pod

## SSH into pods in kubectl
<link>https://kubernetes.io/docs/tasks/debug-application-cluster/get-shell-running-container/</link>

try /bin/sh if bash does't work

## SSH into nodes in minikube
generally, if you want to ssh into nodes, first run:

```bash
kubectl describe nodes

ssh docker@<ip-internal-address>
```

for minikube, password is "tcuser", You can also

```bash
minikube ssh
```


## Reference
<link>https://medium.com/@betz.mark/understanding-resource-limits-in-kubernetes-memory-6b41e9a955f9</link>

