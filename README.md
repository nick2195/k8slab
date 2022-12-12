## K8s lab using kind

**Output from creating a kind cluster

kind create cluster --name k8s --config k8s.yaml
Creating cluster "k8s" ...
 ✓ Ensuring node image (kindest/node:v1.25.3) 🖼
 ✓ Preparing nodes 📦 📦 📦  
 ✓ Writing configuration 📜 
 ✓ Starting control-plane 🕹️ 
 ✓ Installing CNI 🔌 
 ✓ Installing StorageClass 💾 
 ✓ Joining worker nodes 🚜 
Set kubectl context to "kind-k8s"
You can now use your cluster with:

kubectl cluster-info --context kind-k8s

Have a nice day! 👋
root@book:/home/nick/k8slab# kubectl get nodes
NAME                STATUS   ROLES           AGE   VERSION
k8s-control-plane   Ready    control-plane   53s   v1.25.3
k8s-worker          Ready    <none>          32s   v1.25.3
k8s-worker2         Ready    <none>          32s   v1.25.3



***Output after deployment 
kubectl get pods
NAME                                    READY   STATUS    RESTARTS   AGE
zone-spread-topology-64d7595646-6v6rc   1/1     Running   0          87s
zone-spread-topology-64d7595646-dt4th   1/1     Running   0          87s
zone-spread-topology-64d7595646-kwdmd   1/1     Running   0          87s
zone-spread-topology-64d7595646-pqz6q   1/1     Running   0          87s
zone-spread-topology-64d7595646-rkpwl   1/1     Running   0          87s
zone-spread-topology-64d7595646-x7qvk   1/1     Running   0          87s
