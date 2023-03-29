Cloud DevOps Engineer Capstone Project
This project represents the successful completion of the last final Capstone project and the Cloud DevOps Engineer Nanodegree at Udacity.

What did I learn?
In this project, I applied the skills and knowledge I developed throughout the Cloud DevOps Nanodegree program. These include:
==>	Using Circle CI to implement Continuous Integration and Continuous Deployment
==> Building pipelines
==>Working with Ansible and CloudFormation to deploy clusters
==>	Building Kubernetes clusters
==> Building Docker containers in pipelines
==> Working in AWS

!https://dl.circleci.com/status-badge/img/gh/chandrababuchavuturi/Udacity_Capstone--Cloud-DevOps/tree/main.svg?style=svg!:https://dl.circleci.com/status-badge/redirect/gh/chandrababuchavuturi/Udacity_Capstone--Cloud-DevOps/tree/main
Access the Application:-

After deployment successful , I have checked the deployment and service as follows:-
The project is a CI/CD pipeline for deploying a machine learning flask app to AWS EKS
run below command to create the clusrt 
eksctl create cluster -f cluster.yaml 

[![CircleCI](https://dl.circleci.com/status-badge/img/gh/chandrababuchavuturi/Udacity_Capstone--Cloud-DevOps/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/chandrababuchavuturi/Udacity_Capstone--Cloud-DevOps/tree/main)

==>
kubectl get pods
NAME                                READY   STATUS    RESTARTS   AGE
capstone-project-66dd4db478-p82sz   1/1     Running   0          14m
capstone-project-66dd4db478-wtph6   1/1     Running   0          3m2s

=for HTML <a href="https://dl.circleci.com/status-badge/redirect/gh/chandrababuchavuturi/Udacity_Capstone--Cloud-DevOps/tree/main"><img src="https://dl.circleci.com/status-badge/img/gh/chandrababuchavuturi/Udacity_Capstone--Cloud-DevOps/tree/main.svg?style=svg"></a>

==>
kubectl get deployments
NAME               READY   UP-TO-DATE   AVAILABLE   AGE
capstone-project   2/2     2            2           48m

==>
kubectl get services
NAME               TYPE        CLUSTER-IP     EXTERNAL-IP   PORT(S)    AGE
capstone-project   ClusterIP   10.100.5.220   <none>        8080/TCP   48m
kubernetes         ClusterIP   10.100.0.1     <none>        443/TCP    69m   
