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
- Added necessary YAML files in the 'deployment' directory and added this path in application.yaml
![alt text](https://github.com/TejaJanakiRam/DevOpsArgoCD/blob/main/resources/argocdui.png)
- Monitored the application deployment status on the cluster through the dashboard
![alt text](https://github.com/TejaJanakiRam/DevOpsArgoCD/blob/main/resources/argocdfinish.png)

# Task 3:
- Changed application's deployment to use the files in 'rollout' directory, specifying canary release strategy with 8 steps
- Initial docker image is 'v1'.
- To trigger a rollout changed the deployment image to 'v2'.
- Monitored the rollout as they followed all the steps mentioned in the mainfests.

# Challenges
- I had trouble with running the Flask application as there is a conflict with the versions being used.
- Solution: Had use the flask version 2.2.2 + werkzeug version 2.3.7 to solve the problem
- I had no idea the workflow of Kubernetes, minikube, ArgoCD
- Solution: Watch several youtube videos to grasp the concepts and install necessary components
- Had trouble deciding between NodePort and LoadBalancer for argoCD server
- Solution: Decided to go with NodePort as it is less complicated
- Had trouble working with argo rollouts as there are limited resources about it.
- Solution: Had to workout the solution though a punishing trial-and-error series.
