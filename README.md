# Canary-Deployment with argo-rollout
A Practical on Canary deployment using argo-rollout      
Canary Deployemt is a DevOps sofware release stategy for releasing a newer version of software to a few group of users initially for a short period time while every other user can come in afterwards.
Canary deployment can be performed with istio and argo-rollout but for the sake of this practical, I will be demonstrating it with argo-rollout

- [*] Create EKS-Cluster and install:[awscli, Terraform, kubectl and eksctl]

- [*] install Argo Rollout on EKS Cluster

```
kubectl create namespace argo-rollouts

kubectl apply -n argo-rollouts -f https://github.com/argoproj/argo-rollouts/releases/latest/download/install.yaml

kubectl apply -n argo-rollouts -f https://github.com/argoproj/argo-rollouts/releases/latest/download/dashboard-install.yaml 

```
![alt text](IMG-Screenshots/Screenshot_20260814_025342.png)

> Since the boardgame is a java application developed with jda17, then we have to install jdk17: `sudo apt install openjdk-17-jre-headless` Maven: `sudo apt install maven` so as to be able to compile and create a jar file.  `mvn clean package` . alson install docker `sudo apt install docker.io` so as to be able to build and ship 
![alt text](IMG-Screenshots/Screenshot_20260814_023046.png)

![alt text](IMG-Screenshots/Screenshot_20260814_022908.png)

![alt text](IMG-Screenshots/Screenshot_20260814_024324.png)

![alt text](IMG-Screenshots/Screenshot_20260814_024400.png)
