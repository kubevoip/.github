<p align="center">
  <img src="https://raw.githubusercontent.com/kubevoip/kubevoip/main/assets/logo.svg" alt="KubeVoIP logo" width="120">
</p>

# KubeVoIP

KubeVoIP is a Kubernetes-native SIP and VoIP platform.

It uses Kubernetes APIs for Kamailio gateways, RTPengine media relays, Asterisk
application pods, and PostgreSQL-backed routing for SIP users, trunks, dial
policies, and call routes.

## Start here

- Website: [kubevoip.com](https://kubevoip.com)
- Documentation: [docs.kubevoip.com](https://docs.kubevoip.com)
- Platform repository: [kubevoip/kubevoip](https://github.com/kubevoip/kubevoip)
- Quickstart: [Kubernetes VoIP quickstart](https://docs.kubevoip.com/getting-started/quickstart/)

## Repositories

- [`kubevoip`](https://github.com/kubevoip/kubevoip): operator, CRDs, Helm chart, examples, docs automation, and integration tests.
- [`kubevoip-kamailio`](https://github.com/kubevoip/kubevoip-kamailio): Kamailio runtime image.
- [`kubevoip-rtpengine`](https://github.com/kubevoip/kubevoip-rtpengine): RTPengine runtime image.
- [`kubevoip-asterisk`](https://github.com/kubevoip/kubevoip-asterisk): Asterisk runtime image.
- [`website`](https://github.com/kubevoip/website): landing site for kubevoip.com.
- [`docs`](https://github.com/kubevoip/docs): documentation site for docs.kubevoip.com.

## Install

```bash
helm install kubevoip oci://ghcr.io/kubevoip/charts/kubevoip \
  --namespace telephony --create-namespace
```

See the documentation for the current chart version and full quickstart.

## Security

Please report security issues through the platform repository:
[github.com/kubevoip/kubevoip/security](https://github.com/kubevoip/kubevoip/security).
