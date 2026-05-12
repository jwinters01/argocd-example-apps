# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 638bc9e097eded87d177876a0bacbefe9aec40c8
helm template . --name-template staging-helm-guestbook --namespace staging --include-crds
```
