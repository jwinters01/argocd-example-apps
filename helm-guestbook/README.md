# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout c713983a9449e560acbcddd7e19f1e6340f5db64
helm template . --name-template prod-helm-guestbook --include-crds
```
