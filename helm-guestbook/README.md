# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout da1305a48595cca86676cbf4d89261e3211b8220
helm template . --name-template staging-helm-guestbook --namespace staging --include-crds
```
