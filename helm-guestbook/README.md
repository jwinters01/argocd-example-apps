# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout db716d93bd16c877add0c62b1d3f0d54e1df31ce
helm template . --name-template prod-helm-guestbook --include-crds
```
