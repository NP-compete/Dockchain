# The dockchain

Create a blockchain in a docker container, because all problems are solvable with containers and blockchains.

## Usage

### Docker

```shell
docker run --rm --name dockchain sohamdutta0109/dockchain
```

### Kubernetes

```shell
kubectl apply -f https://raw.githubusercontent.com/NP-compete/Dockchain/master/k8s-deployment.yaml
```


## Options

Opts are set via environment variables

| Environment Variable | Type   | Default    | Description                               |
|----------------------|--------|------------|-------------------------------------------|
| `WAIT_PERIOD`        | number | `1`        | Seconds between adding blocks             |
| `EXIT_COUNT`         | number | `Infinite` | How many blocks to create before exiting  |

### Sample config

```shell
docker run --rm -e EXIT_COUNT=20 -e WAIT_PERIOD=2 --name dockchain sohamdutta0109/dockchain
```
