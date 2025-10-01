# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout efb5f76eb543ea7a41fe0ce138d883b714307561
helm template . --name-template development-helm-guestbook --include-crds
```
