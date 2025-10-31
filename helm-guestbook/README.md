# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 6d1cba5a77606be3ccba92130f84077af19d986a
helm template . --name-template development-helm-guestbook --include-crds
```
