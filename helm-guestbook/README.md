# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout be29eef7da2052056ed90ef24c4dcd1371b8b4b8
helm template . --name-template dev-helm-guestbook --namespace development --include-crds
```
