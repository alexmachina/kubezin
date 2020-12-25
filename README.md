# Kubernetesinho básico
```bash
# Redis
kubectl create -f postgres-deploy.yaml
kubectl create -f postgres-service.yaml

# Postgres
kubectl create -f redis-deploy.yaml
kubectl create -f redis-service.yaml

# Voting app
kubectl create -f voting-app-deploy.yaml
kubectl create -f voting-app-service.yaml

# Result app
kubectl create -f result-app-deploy.yaml
kubectl create -f result-app-service.yaml

# Worker app
kubectl create -f worker-app-deploy.yaml

# Obtendo URLs
minikube service voting-service --url
minikube service result-service --url

# Escalando a bagaça
kubectl scale deployment voting-app-deploy --replicas=3
```