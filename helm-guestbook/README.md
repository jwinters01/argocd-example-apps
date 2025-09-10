# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 0d521c6e049889134f3122eb32d7ed342f43ca0d
helm template . --name-template staging-helm-guestbook --include-crds
```
