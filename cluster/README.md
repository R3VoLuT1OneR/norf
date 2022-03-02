# Cluster for DDOS
We need to setup Kubernetes cluster to run the DDOS on it.

For Ubuntu you can use:
```shell
sudo snap install microk8s --classic
```

Setup the needed addons:
```shell
microk8s enable dns dashboard
```

Run next command to get the kubernetes config that we must set to setup local `kubectl` context.

```shell
microk8s config
```

Copy the config into `~/.kube/config` if it is not exists or copy section by section if you have a cluster contexts already.