# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 7b76b4112e6afe6284c88887b8dfc7932bb50636
helm template . --name-template prod-helm-guestbook --namespace prod --include-crds
```
