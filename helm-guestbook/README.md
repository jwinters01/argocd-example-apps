# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 41d245b84e8ce4063b551e640313fc20d021c2b2
helm template . --name-template helm-guestbook-demo --namespace helm-guestbook-demo --include-crds
```
