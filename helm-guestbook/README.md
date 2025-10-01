# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout c1d27fe379d2d758e20d3f0cddde98497e8a7a87
helm template . --name-template development-helm-guestbook --include-crds
```
