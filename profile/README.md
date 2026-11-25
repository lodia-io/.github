<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="lodia-logo-white.svg">
    <img src="lodia-logo.svg" width="140" alt="Lodia">
  </picture>
</p>

Lodia runs Kubernetes control planes as pods on a management cluster, one per tenant cluster, and worker nodes anywhere join them with `kubeadm`.
Each control plane is one `ControlPlane` object: a set of Deployments with an etcd of its own.

The first release is `v0.1.0-alpha.1`, and phase 3 of the [roadmap](https://github.com/lodia-io/lodia/blob/main/docs/roadmap.md) is under way.

```sh
helm install lodia oci://ghcr.io/lodia-io/charts/lodia --version 0.1.0-alpha.1 -n lodia-system --create-namespace
```

- [lodia](https://github.com/lodia-io/lodia): the operator and its Helm chart; [the docs](https://github.com/lodia-io/lodia/blob/main/docs/README.md) and [why it is built this way](https://github.com/lodia-io/lodia/tree/main/docs/decisions)
- [cluster-api-provider-lodia](https://github.com/lodia-io/cluster-api-provider-lodia): the Cluster API control plane provider
- [Contributing](https://github.com/lodia-io/lodia/blob/main/CONTRIBUTING.md), [security policy](https://github.com/lodia-io/lodia/blob/main/SECURITY.md), [code of conduct](https://github.com/lodia-io/lodia/blob/main/CODE_OF_CONDUCT.md)
- hello@lodia.io
