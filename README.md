# k8s-yaml-manifests
Manifest files to setup Kubernetes resources

## Instructions for setting up infra using kubernetes
1. Install Kubernetes
2. Install minikube
3. Run minikube start
4. Generate registry access secret using kubectl create secret docker-registry (name)
5. Run kubectl get secret (name) --output=yaml
6. Copy output of previous command to secrets.yaml
7. Run kubectl -f apply secrets.yaml
8. Run kubectl -f apply config.yaml
9. Run kubectl -f apply pod.yaml
