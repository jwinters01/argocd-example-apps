# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 6c40e4f47d6e2e82dc8817b6c592ac9ad335890b
helm template . --name-template staging-helm-guestbook --include-crds
```
