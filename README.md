# Argocd-deployment

#This is customize repo link
https://argo-cd.readthedocs.io/en/stable/operator-manual/installation/#kustomize

Step-1: Create namespace
k create ns argocd

Step-2: Create directory
mkdir argocd and then cd argocd


#This is my kustomize repo link 
https://argo-cd.readthedocs.io/en/stable/operator-manual/installation/#kustomize

Step-1: Create namespace

k create ns argocd

Then just make a directory argocd or with any name, then go to that directory
cd argocd
Create a file name kustomization.yaml. Then apply

kubectl apply -k .
