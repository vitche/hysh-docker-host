# HyperShell Docker Host management container
This container implements a Docker container suitable for
provisioning the whole Docker-based micro-service runtime
by controlling the Docker Host machine.

## How to start your agent
Can be started with:
```shell
docker run -dit --restart always --name hysh-docker-host -e "CHAINCODE_ID_NAME=48a80f9f705b4777af9216e69e1a85ba" -v /var/run/docker.sock:/var/run/docker.sock vitche/hysh-docker-host
```
- The agent identifier is specified using the "CHAINCODE_ID_NAME" environment variable.
- Access to the Docker Host Docker daemon is granted by mounting the Docker socket into the container.
