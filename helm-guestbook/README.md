# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 7855e35b8b1e8446b8c47f39a07eb6d5e0af12f0
helm template . --name-template prod-helm-guestbook --namespace prod --include-crds
```
