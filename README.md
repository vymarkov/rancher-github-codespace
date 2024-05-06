# rancher-github-codespace


### Minikube

```bash
minikube start --kubernetes-version=v1.28
```

```bash
helm repo add jetstack https://charts.jetstack.io
```

```bash
helm install cert-manager jetstack/cert-manager --namespace=cert-manager --version 1.10.2 --set installCRDs=true
```

```
helm repo add rancher-latest https://releases.rancher.com/server-charts/latest
```

```bash
kubectl create ns cattle-system
```

```bash
helm install rancher rancher-latest/rancher --namespace=cattle-system --set hostname=didactic-zebra-wrgqr54q5rh5xg5.github.dev --set bootstrapPassword=password --wait --timeout=10m
```