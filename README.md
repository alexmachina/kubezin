# Kubernetesinho básico
```bash
# Redis
kubectl create -f postgres-pod.yaml
kubectl create -f postgres-service.yaml

# Postgres
kubectl create -f redis-pod.yaml
kubectl create -f redis-service.yaml

# Voting app
kubectl create -f voting-app-pod.yaml
kubectl create -f voting-app-service.yaml

# Result app
kubectl create -f result-app-pod.yaml
kubectl create -f result-app-service.yaml

# Worker app
kubectl create -f worker-app-pod.yaml

# Obtendo URLs
minikube service voting-service --url
minikube service result-service --url
```