# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout c3d3757e2447956573432b7eb043550c83cb4197
helm template . --name-template dev-helm-guestbook --namespace development --include-crds
```
