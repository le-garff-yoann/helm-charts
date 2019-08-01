# mojochat

This chart deploys [mojochat](https://github.com/le-garff-yoann/mojochat).

## TL;DR;

```bash
helm install le-garff-yoann/mojochat
```

## Prerequisites

* Kubernetes 1.4+ with Beta APIs enabled.

## Installing the Chart

To install the chart with the release name `mojochat-1`:

```bash
helm install le-garff-yoann/mojochat --name mojochat-1
```

## Installing with Ingress

```bash
helm install le-garff-yoann/mojochat \
    --name mojochat-1 \
    --set ingress.enabled=true \
    --set ingress.hosts[0]=mojochat-1.default.mydomain.io
```

## Uninstalling the Chart

To uninstall/delete the `mojochat-1` deployment:

```bash
helm delete mojochat-1
```
