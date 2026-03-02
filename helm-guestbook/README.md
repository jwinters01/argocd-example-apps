# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout 3805ea84283d0f808eb7b6f53a9c6358676dd44a
helm template . --name-template staging-helm-guestbook --namespace staging --include-crds
```
