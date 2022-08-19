# Backlog

## Initial stage

Implement GitOps with ArgoCD and Crossplane.

![](img/pocGitOps-sync.jpg)

## CI/CD stage

Add a CI/CD pipeline with Argo Events and Argo Workflows to run Terratest verifications and rollback failing releases.

Two repositories will be used. One will act as input interface (where users will have access), and then a CI/CD pipeline will update another repo that will only hold the GitOps state. In case the pipeline fails it will try to rollback the input from the user.

![](img/pocGitOps-components.jpg)

## Improvements stage

- Replace Argo Events and Argo Workflows with Tekton.