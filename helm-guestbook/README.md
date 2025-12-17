# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 96d1912a0972aff8b8c8aa10871b3d87721d88b2
helm template . --name-template perf-helm-guestbook --include-crds
```
