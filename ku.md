# Create Yaml file (nginx-deployment.yaml)
```
apiVersion: apps/v1
kind: Deployment
metadata:
  name: nginx-deployment
spec:
  replicas: 18
  selector:
    matchLabels:
      app: nginx
  template:
    metadata:
      labels:
        app: nginx
    spec:
      containers:
      - name: nginx
        image: nginx:latest
        ports:
        - containerPort: 80

```

- `winget install kubernetes.kubectl`
- `kubectl version --client`
- `kubectl apply -f nginx-deployment.yaml`
- `kubectl expose deployment nginx-deployment --type=LoadBalancer --port=80`
- `kubectl get services`
- `kubectl get pods`
