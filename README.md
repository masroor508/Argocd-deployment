# Argocd-deployment

#This is my kustomize repo link 
https://argo-cd.readthedocs.io/en/stable/operator-manual/installation/#kustomize

Step-1: Create namespace

k create ns argocd

Then just make a directory argocd or with any name, then go to that directory
cd argocd
Create a file name kustomization.yaml
Then paste the below kustomize content

apiVersion: kustomize.config.k8s.io/v1beta1

kind: Kustomization

namespace: argocd

resources:

- https://raw.githubusercontent.com/argoproj/argo-cd/v2.7.2/manifests/install.yaml

:wq

k apply -k .



