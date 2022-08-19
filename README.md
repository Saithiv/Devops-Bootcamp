# Devops-Bootcamp
### Kanban board project

#### First step: 
[Workflow](https://trello.com/invite/b/vmpwrOsd/be1bd1241d712b3a96839d2e7ef353c2/devops) for the given acceptance criteria:
*         Clone the web application 
          $git clone https://github.com/swarajspatil158/to-do-app.git
          
* 		Create a docker image of the web application
          Dockerfile
          
* 		Push our docker image to Dockerhub
          $ docker tag saithivyah/teamsr:latest saithivyah/sr-todo 
          $ docker push saithivyah/sr-todo
          
* 		Run as docker image
          $ docker run -i -p 3000:80 saithivyah/sr-todo
          
* 		Implemented in minikube as local deployment
          deployment.yaml
          service.yaml
          
          $ kubectl apply -f deployment.yaml
          $ kubectl apply -f service.yaml
          
          $ kubectl get nodes -o wide
          $ kubectl get svc
          
          http://<node external IP> : <node-port>

* 		Create a VPC with public and private subnets for our EKS Cluster
          main.tf - includes creation of Vpc, 
* 		Create a Kubernetes Cluster
* 		Create Kubernetes workers(public and private workers)
* 		Deploy our web application on Kubernetes



     
