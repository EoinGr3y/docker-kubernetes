# kubernetes-multi-container
Kubernetes multi container task application from [udemy docker course](https://www.udemy.com/course/docker-kubernetes-the-practical-guide/)

This application is composed of 4 components;
- auth-api - token verification
- frontend - simple ui for adding/viewing tasks
- tasks-api - backend api for task creation/retrieval
- users-api - backend api for user sign up/login

## Prerequisites
Note that you must have both minikube and kubectl installed to run this locally.

Ensure minikube is running with the command `minikube status`. If it is not running you can start it with the command `minikube start --driver=virtualbox`
You can then create the kubernetes services & deployments by running the command `kubectl apply -f auth-deployment.yaml -f auth-service.yaml -f frontend-deployment.yaml -f frontend-service.yaml -f tasks-deployment.yaml -f tasks-service.yaml -f users-deployment.yaml -f users-service.yaml` from the kubernetes directory.