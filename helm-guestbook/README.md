# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout b6f78ea9e887b87a595093817bb614d34ff27b65
helm template . --name-template prod-helm-guestbook --include-crds
```
