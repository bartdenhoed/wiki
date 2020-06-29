# Docker Development

> https://medium.com/@yutafujii_59175/a-complete-one-by-one-guide-to-install-docker-on-your-mac-os-using-homebrew-e818eb4cfc3

### Install Docker
- `brew install docker` (Client)
- `brew install docker-machine` (Daemon)
- `brew cask install virtualbox` (VM)

### Create Virtual Machine
- New VM: `docker-machine create --driver virtualbox [vm-name]`
- List VM: `docker-machine ls`

### Activate Docker
- `docker-machine env [vm-name]`
- `eval $(docker-machine env [vm-name]`

### Testing
- `docker run hello-world`

### Stop Virtual Machine
- `docker-machine stop [vm-name]`
