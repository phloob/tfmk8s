# tfm k8s
Goofin' with k8s and terraform

# Guide
https://learn.hashicorp.com/tutorials/terraform/kubernetes-provider

*assumes docker/docker desktop already installed*
#  Install / setup steps
1. brew install kind
2. kind create cluster --name terraform-learn --config kind-config.yaml
3. kind get clusters
4. kubectl cluster-info --context kind-terraform-learn
5. kubectl config current-context
6. kubectl config use-context kind-terraform-learn
7. terraform init
8. terraform apply
9. kubectl get deployments
10. kubectl get services
11. terraform destroy
12. kind delete cluster --name terraform-learn

# Documentation
https://registry.terraform.io/providers/hashicorp/kubernetes/latest/docs


# Potential goals?

- add webpage content for nginx containers?

  -  https://kubernetes.io/docs/concepts/containers/images/
- tiered clusters with different webapp version?
