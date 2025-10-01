# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout e8cadda4fb025eff15c86727a841ee3a36aa3c92
helm template . --name-template staging-helm-guestbook --include-crds
```
