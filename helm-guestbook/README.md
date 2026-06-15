# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 8e23b875ddb5cc1bff80f263606442b8c1cdc9ac
helm template . --name-template staging-helm-guestbook --namespace staging --include-crds
```
