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

## Exercise 2: Multi-Container Pod with Shared Volume
- Created a pod with nginx and content-generator containers
- Implemented shared volume communication
- Used emptyDir volume type
- Demonstrated sidecar container pattern

### Commands Used
```bash
kubectl apply -f multi-container-pod.yaml
kubectl get pods
kubectl exec multi-container-pod -c nginx -- curl localhost:80
```

### Learning Points
- Volume sharing between containers
- Container communication patterns
- Pod lifecycle management
- Sidecar container pattern implementation
