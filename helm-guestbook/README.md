# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout c3e813637c23ea2d9d2185d29e1f0bbe864ba5e0
helm template . --name-template prod-helm-guestbook --namespace prod --include-crds
```
