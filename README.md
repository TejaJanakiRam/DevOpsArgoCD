# DevOpsArgoCD+ArgoRollouts Assignment Process
# Task 1:
I created this repository to host both the source code of the application and also the kubernetes manifests.
- Created a Kubernetes cluster using minikube
- Installed kubectl to control the minikube cluster
- Installed Argo CD in the cluster using official documentation
- Installed Argo Rollouts in the cluster 
![alt text](https://github.com/TejaJanakiRam/DevOpsArgoCD/blob/main/resources/argocd.png)
# Task 2:
- First created a simple web application using Flask and python
![alt text](https://github.com/TejaJanakiRam/DevOpsArgoCD/blob/main/resources/Flask.png)
- Built a docker image using 'docker build' command (Find configuration in Dockerfile)
- Pushed it to the repo tejdocker32/argocd on DockerHub
- Included the docker repo in kubernetes manifests
- Completed ArgoCD setup and used decoded credentials to login
![alt text](https://github.com/TejaJanakiRam/DevOpsArgoCD/blob/main/resources/argocdui.png)
- Monitored the application deployment status on the cluster through the dashboard
![alt text](https://github.com/TejaJanakiRam/DevOpsArgoCD/blob/main/resources/argocdfinish.png)
  
