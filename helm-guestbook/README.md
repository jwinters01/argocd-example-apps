# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 1a1b1341eabd4c6f8b253832f5eadc496974b1e9
helm template . --name-template staging-helm-guestbook --namespace staging --include-crds
```
