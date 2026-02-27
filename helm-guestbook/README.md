# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout f7a48f1ca2f1cc3da3f39ea5468f03c6dcc61401
helm template . --name-template dev-helm-guestbook --namespace development --include-crds
```
