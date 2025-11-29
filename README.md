# Gogs Helm Chart

lightweight helm chart for [gogs](https://gogs.io/)

mostly taken from [drabo/gogs](https://github.com/drabo/gogs) but customized specifically to use in my homelab.

[Repo Link](https://github.com/chr0n1x/gogs-helm-chart)

# Why?

Couldn't find a light-weight enough helm chart for gogs. Decided to make my own & have the release process be public via github actions.

# Disclaimer

This chart is written to be used _WITH_ an ingress/api-gateway of your choice. As such, I provide no config values for auto-creating an ingress object.

For an example of this chart being used w/ a [traefik IngressRoute](https://doc.traefik.io/traefik/reference/routing-configuration/kubernetes/crd/http/ingressroute/), check out [my wrapper chart for my homelab](https://github.com/chr0n1x/rpi-talos/tree/main/k8s/argocd-deploy/gogs)

# Contributions?

Welcome! Feel free to raise a PR.

# Usage

```sh
helm repo add gogs https://chr0n1x.github.io/gogs-helm-chart
helm install gogs gogs
```

