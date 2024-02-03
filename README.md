_**Author: @Jaz-3-0**_

# About

Setting up a basic hyperledger fabric 2.0 network

## Prerequisites

- cURL installed
- golang installed
- python v3 installed
- node.js LTS installed
- npm LTS installed

### Getting started - full guide

```sh
export GOPATH=$HOME/go
export PATH=$PATH:$GOPATH/bin
source ~/.bashrc || . ~/.bashrc || vim ~/.bashrc
```

**Installation**

`Docker Engine`

```sh

# Add Docker's official GPG key:
sudo apt-get update
sudo apt-get install ca-certificates curl
sudo install -m 0755 -d /etc/apt/keyrings
sudo curl -fsSL https://download.docker.com/linux/ubuntu/gpg -o /etc/apt/keyrings/docker.asc
sudo chmod a+r /etc/apt/keyrings/docker.asc

# Add the repository to Apt sources:
echo \
  "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.asc] https://download.docker.com/linux/ubuntu \
  $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
  sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
sudo apt-get update

```

```sh
# Install the latest docker packages

sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin
```

```sh
# Verify that the docker engine installation is succesful
sudo docker run hello-world
```

```sh

# To uninstall the docker engine
sudo apt-get purge docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin docker-ce-rootless-extras

# Delete all the images, containers and volumes

sudo rm -rf /var/lib/docker
sudo rm -rf /var/lib/containerd
```

`Install docker-compose from docker - snap`

```sh
# Install it with docker
sudo snap install docker
# docker will come with it in this case
```

`Or install it separately`

```sh
# Install it separately
sudo apt install docker-compose
```

`Verify the versions`

```sh

curl --version
npm --version
node --version
docker version
docker-compose version
go --version
python3 --version

```

-------

@Jaz-3-0
