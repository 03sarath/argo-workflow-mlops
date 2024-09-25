# Getting started with Argo workflow on minikube 

### Prerequisites
1. Docker Desktop
2. Minikube installed

### Install Argo Workflows¶

```
minikube start
```
```
kubectl create namespace argo
```
```
kubectl apply -n argo -f "https://github.com/argoproj/argo-workflows/releases/download/v3.5.11/quick-start-minimal.yaml"

```
You can find your latest version of argo-workflow here https://github.com/argoproj/argo-workflows/releases/

### Access Argo Workflow Ui
1. Forward the Server's port to access the UI:
```
kubectl -n argo port-forward service/argo-server 2746:2746
```
2. Navigate your browser to https://localhost:2746.


