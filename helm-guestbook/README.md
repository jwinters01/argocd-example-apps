# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 796c3887be721a93c5d30e518f9a118b6a0a307e
helm template . --name-template gamma-helm-guestbook --namespace gamma --include-crds
```
