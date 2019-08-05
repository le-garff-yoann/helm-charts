# jitsi-meet

This chart deploys a basic setup of [Jitsi Meet](https://jitsi.org/jitsi-meet/).

The images are pulled from [hub.docker.com/u/jitsi](https://hub.docker.com/u/jitsi).

## TL;DR;

```bash
helm install le-garff-yoann/jitsi-meet
```

## Prerequisites

* Kubernetes 1.4+ with Beta APIs enabled.

## Installing the Chart

To install the chart with the release name `jitsi-meet-1`:

```bash
helm install le-garff-yoann/jitsi-meet --name jitsi-meet-1
```

## Installing with Ingress

```bash
helm install le-garff-yoann/jitsi-meet-1 \
    --name jitsi-meet-1 \
    --set ingress.enabled=true \
    --set ingress.hosts[0]=jitsi-meet-1.default.mydomain.io
```

## Uninstalling the Chart

To uninstall/delete the `jitsi-meet-1` deployment:

```bash
helm delete jitsi-meet-1
```
