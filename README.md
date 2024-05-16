# Argocd-deployment

#This is customize repo link
https://argo-cd.readthedocs.io/en/stable/operator-manual/installation/#kustomize

Step-1: Create namespace
k create ns argocd

Step-2: Create directory
mkdir argocd and then cd argocd

cd argocd
Create a file name kustomization.yaml. Then apply

kubectl apply -k .

Step-3: Verify the pods in argocd namespace
k get pod -n argocd

Step-4: Setup the DNS url
k get svc -n argocd
argocd-server  service name need to modify
kubectl edit svc argocd-server -n argocd
change the type: ClusterIP to LoadBalancer