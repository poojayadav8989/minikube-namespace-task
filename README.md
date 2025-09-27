# Minikube Namespace Task

## Steps Performed

1. Installed Docker, Minikube, and kubectl using Homebrew.
2. Started Minikube cluster:
   ```bash
Verified cluster and namespaces:

bash
Copy code
kubectl get nodes
kubectl get namespaces
Created namespaces dev and test:

bash
Copy code
kubectl create namespace dev
kubectl create namespace test
Deployed nginx pod inside dev namespace:

bash
Copy code
kubectl run nginx-pod --image=nginx -n dev
kubectl get pods -n dev
Deleted test namespace:

bash
Copy code
kubectl delete namespace test
Screenshots
Screenshots are available inside the screenshots/ folder.

kube1.png

kube2.png

Tools Used
Docker

Minikube

kubectl

macOS (via Homebrew)
