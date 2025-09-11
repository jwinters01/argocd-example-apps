# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 7cbc03775792ab10a834ac1a7bb75727b92d39eb
helm template . --name-template prod-helm-guestbook --include-crds
```
