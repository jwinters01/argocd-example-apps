# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout da77389b5785469ce7c5b63e97232a9f3aa18bab
helm template . --name-template prod-helm-guestbook --namespace prod --include-crds
```
