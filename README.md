# noops-operator
This operator does nothing. Its purpose is to reproduce an issue when communication with the API server results in an I/O timeout.

### Running on the cluster
1. Build and push your image to the location specified by `IMG`:

```sh
make docker-build docker-push IMG=<some-registry>/noops-operator:tag
```

2. Deploy the controller to the cluster with the image specified by `IMG`:

```sh
make deploy IMG=<some-registry>/noops-operator:tag
```

### Undeploy controller
Undeploy the controller from the cluster:

```sh
make undeploy
```
