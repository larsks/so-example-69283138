This repository accompanies
<https://stackoverflow.com/a/69283807/147356>.

To deploy this example:

```
kubectl apply -k .
```

This will create a namespace `postgres-example` and deploy the example
application into it.

Or, if your `kubectl` is too old, install [kustomize][] and then:

```
kustomize build | kubectl apply -f-
```

When you're done and want to clean up:

```
kubectl delete -k .
```

[kustomize]: https://kustomize.io/
