# Installation


#### Create separate argocd namespace

```http
  kubectl create namespace argocd
```

#### Deploy argocd 

```http
  kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml
```

# Setup


#### Get all information about argocd 

```http
  kubectl get all -n argocd
```

#### Port foward for access web gui

```http
  kubectl port-forward service/argocd-server -n argocd 8080:443
```
