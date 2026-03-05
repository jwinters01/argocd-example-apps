# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 7de6542e09b0f69084817e2b7b6d6c4372a20756
helm template . --name-template dev-helm-guestbook --namespace development --include-crds
```
