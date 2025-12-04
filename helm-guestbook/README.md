# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 03d422c2d28f2f9116603d8859c780312cc0ffde
helm template . --name-template qal-helm-guestbook --include-crds
```
