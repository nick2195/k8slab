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
