# Deployment Practice

## Exercise 1: Basic Nginx Deployment
- Created a deployment with 3 replicas
- Used nginx:1.14.2 image
- Exposed port 80

### Commands Used
```bash
kubectl apply -f nginx-deployment.yaml
kubectl get deployments
kubectl get pods
```

### Learning Points
- Understanding deployment structure
- Managing replicas
- Pod template configuration
