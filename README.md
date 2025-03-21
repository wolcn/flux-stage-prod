### Second scenario
Two environments, two namespaces and one repo

If `yq` is installed, a useful way to check for updates is:
```
kubectl -n dev get deploy kcheck -oyaml | yq .metadata.generation
```
