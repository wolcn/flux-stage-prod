### Second scenario
Two environments, two namespaces and one repo

If `yq` is installed, a useful way to check for updates is:
```
kubectl -n fluxdemo-stage get deploy kcheck -oyaml | yq .metadata.generation
kubectl -n fluxdemo-prod get deploy kcheck -oyaml | yq .metadata.generation
```
