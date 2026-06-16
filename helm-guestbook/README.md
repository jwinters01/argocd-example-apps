# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout a7bf50f1ea0e6164f8ea9726102ed6ad29841e0e
helm template . --name-template prod-helm-guestbook --namespace prod --include-crds
```
