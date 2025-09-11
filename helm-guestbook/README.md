# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 8c3f42d554b7ae1561bd34bcd8db328c5420d1d4
helm template . --name-template staging-helm-guestbook --include-crds
```
