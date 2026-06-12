# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 292ccf53b1b0a02b96a4c942e491d0e23443cef5
helm template . --name-template prod-helm-guestbook --namespace prod --include-crds
```
