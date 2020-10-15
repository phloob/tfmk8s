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

http://nginx.org/en/docs/beginners_guide.html

https://docs.docker.com/registry/

https://hub.docker.com/_/nginx

# Potential goals?

- add webpage content for nginx containers?

  -  https://kubernetes.io/docs/concepts/containers/images/
- tiered clusters with different webapp version?

Long term: immutable static webpage infrastructure

# Next steps:

1. Setup docker registry for app container image
2. Create new repo(?) for container images?

    - Use image = "nginx:1.7.8" as a boilerplate 
3. Start with a basic edit to the html file /root/data
4. Add CI/CD!
5. Deploy into cloud environment?
