# Canary-Deployment with argo-rollout
A Practical on Canary deployment using argo-rollout      
Canary Deployemt is a DevOps sofware release stategy for releasing a newer version of software to a few group of users initially for a short period time while every other user can come in afterwards.
Canary deployment can be performed with istio and argo-rollout but for the sake of this practical, I will be demonstrating it with argo-rollout

- [*] Create EKS-Cluster and install:[awscli, Terraform, kubectl and eksctl]

- [*] install Argo Rollou on EKS Cluster

```
kubectl create namespace argo-rollouts

kubectl apply -n argo-rollouts -f https://github.com/argoproj/argo-rollouts/releases/latest/download/install.yaml

kubectl apply -n argo-rollouts -f https://github.com/argoproj/argo-rollouts/releases/latest/download/dashboard-install.yaml 

```
