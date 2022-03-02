# No RF
Just an experiment with TOR network and DDOS tools.

## TOR Proxy
We have a HELM chart to deploy to use the TOR proxy.

```shell
kubectl create namespace torproxy
helm upgrade --install --namespace torproxy torproxy ./torproxy
```

## Helm Chart
Install next helm chart to run ddos in kubernetes.

```shell
helm upgrade --install norf ./ddosify
```