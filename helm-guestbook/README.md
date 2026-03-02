# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 072136ef57b82fca1c10ba1de23cbc9526901d9d
helm template . --name-template prod-helm-guestbook --namespace prod --include-crds
```
