# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout a0d3f48841aab6086995e40e11eaa087f0f2a9b1
helm template . --name-template staging-helm-guestbook --namespace staging --include-crds
```
