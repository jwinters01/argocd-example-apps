# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 9104731fe238da2314b0a1728943ef1f13e95117
helm template . --name-template prod-helm-guestbook --namespace prod --include-crds
```
