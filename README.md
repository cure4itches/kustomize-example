# kustomize-example
A simple Nginx application with kustomize

## How to run
### dev
```shell
kubectl create namespace dev
kustomize overlay/dev | kubectl -n dev apply -f -
```
### prod
```shell
kubectl create namespace prod
kustomize overlay/prod | kubectl -n prod apply -f -
```
