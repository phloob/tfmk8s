# tfm k8s
Goofin' with k8s and terraform

#  Install / setup steps
1. brew install kind
2. curl https://raw.githubusercontent.com/hashicorp/learn-terraform-deploy-nginx-kubernetes-provider/master/kind-config.yaml --output kind-config.yaml
3. kind create cluster --name terraform-learn --config kind-config.yaml
4. kind get clusters
5. kubectl cluster-info --context kind-terraform-learn
6. mkdir learn-terraform-deploy-nginx-kubernetes
7. cd learn-terraform-deploy-nginx-kubernetes
8. touch kubernetes.tf <content>
9. kubectl config current-context
10. kubectl config use-context kind-terraform-learn
11. terraform init
12. terraform apply
13. kubectl get deployments
14. kubectl get services
15. terraform destroy
16. kind delete cluster --name terraform-learn
