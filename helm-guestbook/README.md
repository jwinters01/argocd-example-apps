# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 35b02c97531ed01db44049a3dc800dab8a1f0ba6
helm template . --name-template alpha-helm-guestbook --namespace alpha --include-crds
```
