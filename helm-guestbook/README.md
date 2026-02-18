# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout a828517a751e6a505b2b538cd9d7a163ccb33c2b
helm template . --name-template prod-helm-guestbook --namespace prod --include-crds
```
