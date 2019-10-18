# The dockchain

Create a blockchain in a docker container, because all problems are solvable with containers and blockchains.


## Options

Opts are set via environment variables

| Environment Variable | Type   | Default    | Description                               |
|----------------------|--------|------------|-------------------------------------------|
| `WAIT_PERIOD`        | number | `1`        | Seconds between adding blocks             |
| `EXIT_COUNT`         | number | `Infinite` | How many blocks to create before exiting  |