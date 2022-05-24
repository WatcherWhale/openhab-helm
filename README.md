# openHAB - Helm Chart

This repo contains all charts to deploy openHAB in a kubernetes cluster.

## Install openHAB with helm

```console
$ helm repo add openhab-helm https://watcherwhale.github.io/openhab-helm/
$ helm repo update

$ helm install openhab openhab-helm/openhab
```

## Configuration

To configure this chart read through the [values.yaml](./charts/openhab/values.yaml) or the [readme](charts/openhab/README.md) in the opehhab chart.

You can then create a custom `values.yaml` and deploy it:

```console
$ helm install openhab openhab-helm/openhab -f values.yaml
```
