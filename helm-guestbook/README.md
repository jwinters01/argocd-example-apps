# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 82255c8e6ad082f4fed5bfa2eabd3a33d7a9640e
helm template . --name-template alpha-helm-guestbook --namespace alpha --include-crds
```
