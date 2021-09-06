# k8s-voting-app
This is a multi-tier application developed during my studies of kubernetes and how to deploy and maintain an application made of multiple services containers maintained by Kubernetes.

## Running this application in a K8s cluster
- 1: Clone this repository locally
- 2: Navigate to the local repo and run the following commands:
    - kubectl create -f voting-app-deployment.yaml
    - kubectl create -f voting-app-service.yaml
    - kubectl create -f redis-deployment.yaml
    - kubectl create -f redis-service.yaml
    - kubectl create -f postgres-deployment.yaml
    - kubectl create -f postgres-service.yaml
    - kubectl create -f worker-app-deployment.yaml
    - kubectl create -f result-app-deployment.yaml
    - kubectl create -f result-app-service.yaml

The Voting Web app will be available at: http://nodeIpAddress:30004
The results Web app will be available at: http://nodeIpAddress:30005
