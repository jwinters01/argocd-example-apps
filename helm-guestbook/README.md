# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout b99603897d85d9b79c33e8620cd4af584c46fa67
helm template . --name-template dev-helm-guestbook --namespace development --include-crds
```
