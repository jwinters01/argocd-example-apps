# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 1345ea8cef32924aeb4a557f1e638886426cac5a
helm template . --name-template prod-helm-guestbook --namespace prod --include-crds
```
