# Manifest Hydration

To hydrate the manifests in this repository, run the following commands:

```shell
git clone https://github.com/jwinters01/argocd-example-apps
# cd into the cloned directory
git checkout d1b25104ac911cf298ec2c823aa62a779bd8e020
helm template . --name-template staging-helm-guestbook --namespace staging --include-crds
```
