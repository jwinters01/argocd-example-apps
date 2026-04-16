# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout ba8cbafe0979a824f6cbf1621eba53ff30c799dd
helm template . --name-template staging-helm-guestbook --namespace staging --include-crds
```
