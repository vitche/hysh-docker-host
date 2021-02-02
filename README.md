# HyperShell Docker Host management container
This container implements a Docker container suitable for
provisioning the whole Docker-based micro-service runtime
by controlling the Docker Host machine.

## How to start your agent
Can be started with:
```shell
docker run -dit --restart always --name hysh-docker-host-ubuntu -e "CHAINCODE_ID_NAME=48a80f9f705b4777af9216e69e1a85ba" vitche/hysh-docker-host-ubuntu
```
The agent identifier is specified using the "CHAINCODE_ID_NAME" environment variable.