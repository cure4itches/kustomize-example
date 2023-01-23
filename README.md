# kustomize-example
A simple Nginx application with kustomize

## How to run
### dev
```shell
kubectl create namespace dev
kustomize build overlay/dev | kubectl -n dev apply -f -
```
### prod
```shell
kubectl create namespace prod
kustomize build overlay/prod | kubectl -n prod apply -f -
```
