# kubectl-purge-namespace

Delete all resources out of a given namespace. Deletes the following resource types:

- `configmap`
- `deployment.apps`
- `ingress`
- `job`
- `pod`
- `pvc`
- `secret`
- `service`
- `statefulset.apps`

## Usage

Pass the namespace to be deleted:

```sh
kubectl-purge-namespace your-namespace-to-purge
```

You will see a list of resources that will be deleted and must confirm before any deletes occur.

Multiple namespaces can be space delimited:

```sh
kubectl-purge-namespace namespace-a namespace-b namespace-c
```
