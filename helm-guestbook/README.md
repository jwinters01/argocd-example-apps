# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout cd676414ae172aaed87b7b898249e0a6601b9d8b
helm template . --name-template gamma-helm-guestbook --namespace gamma --include-crds
```
