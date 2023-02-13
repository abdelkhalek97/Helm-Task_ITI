# Helm-Task_ITI
This is a mini project aims to deploy redis and python app using helm.<br>
Application : https://github.com/atefhares/DevOps-Challenge-Demo-Code <br>
Image used : https://hub.docker.com/r/ahmednasrhassan/devops-challenge

### Requirments :
- Kubectl cli
- MiniKube

### Before you run any command
edit this **file ("Helm-Task_ITI/python/.vscode/settings.json")** to match configmap.yaml location on your machine . 

### Run these commands while you are in Helm-task_ITI directory:
```
helm install custom-redis redis/
```
```
helm install custom-app python/
```

### To make sure everything is running :
```
kubectl get all
```
### Start minikube tunnel:
```
minikube tunnel
```
**now you can insert ip of the NodePort in your browser and the python app will be up and running.**
