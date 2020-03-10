# This chart installs the Isso comments system on kubernetes

## Prerequisites

* a working HTTP/HTTPS ingress controller such as nginx or traefik
* cert-manager v0.12 or higher installed and configured (including a working cert issuer).

## Installation

```
git clone git@github.com:rouja/isso-chart.git
cp isso-chart/values.yaml custom-values.yml #Edit the custom-values.yml to fit to your env
kubectl create ns isso
helm upgrade -f custom-values.yml --install -n isso isso isso-chart/
```

**WARNING** It's a work in progress. This chart needs improvement.
