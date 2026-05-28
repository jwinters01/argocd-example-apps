# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 32a4f90e4e9622c741545fffea5fa52d8e52ae18
helm template . --name-template dev-helm-guestbook --namespace development --values ./helm-guestbook/values.yaml --values ./helm-guestbook/values-development.yaml --include-crds
```
