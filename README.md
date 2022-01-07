# Kubernetes Objects

Some example (or actually useful for productive use) Kubernetes objects.

Tested on k3s.

## Example

To install a instance called `production` of the `whoami` chart into a new namespace `whoami-helm` and override the default values with your own in `whoami/values-override.yaml` do this:

```
helm install production whoami --create-namespace -n whoami-helm -f whoami/values-override.yaml --kubeconfig /var/lib/rancher/k3s/server/cred/admin.kubeconfig
```
