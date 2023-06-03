# PoC Voting App with K8S

```bash

cd k8s
kubectl create namespace voting-app
kubectl apply -f . --namespace=voting-app
kubectl get all --namespace=voting-app

# To scale the deployments
kubectl scale deployment vote --replicas=5 --namespace=voting-app
kubectl scale deployment result --replicas=5 --namespace=voting-app

# To delete all objects
kubectl delete all --all --namespace voting-app

```
