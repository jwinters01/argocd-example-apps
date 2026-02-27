# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 00edd67d48d432b84a5807444824c41e53713110
helm template . --name-template dev-helm-guestbook --namespace development --include-crds
```
