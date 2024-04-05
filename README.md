# fabric.2.0.net

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
source ~/.bashrc || . ~/.bashrc || vim ~/.bashrc || pico ~/.bashrc
```

_**Installation**_

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

`Some docker images used`

```sh
curl -sSL https://bit.ly/2ysbOFE | bash -s
```

`Installation of hyperledger fabric`

```sh

# update apt packages
sudo apt update
sudo apt upgrade
# create new user(fabric)
sudo adduser fabric
sudo usermod -aG sudo fabric
su - fabric

# Install overall prerequisites
sudo apt-get update
sudo apt-get install git curl docker.io docker-compose nodejs npm python

# start && enable docker
sudo usermod -a -G docker $USER
sudo systemctl start docker
sudo systemctl enable docker
```

`Dealing with platform specific binaries`

```sh
# Make sre you have a latest curl version
# Install it with this command
wget https://github.com/hyperledger/fabric/blob/master/scripts/bootstrap.sh

# Note: You can use this command for any published version of Hyperledger Fabric. Simply replace ‘1.1.0’ with the version identiﬁer of the version you wish to install

# Execute this in the very exact directory

curl -sSL https://goo.gl/6wtTN5 | bash -s <fabric> <fabric-ca> <thirdparty>
curl -sSL https://goo.gl/6wtTN5 | bash -s 1.1.0 1.1.0 0.4.6
```

`Binaries downloaded are`

- cryptogen,
- configtxgen,
- configtxlator,
- peer
- orderer and
- fabric-ca-client

`You may want to add that to your PATH`

```sh
export PATH=<path to download location>/bin:$PATH
```

### `Hyperledger fabric sdks`

- [Hyperledger fabric Node SDK](https://github.com/hyperledger/fabric-sdk-node) and [Node SDK Documentation](https://fabric-sdk-node.github.io)
- [Hyperledger fabric Java SDK](https://github.com/hyperledger/fabric-sdk-node)
- [Hyperledger fabric Python SDK](https://github.com/hyperledger/fabric-sdk-py)
- [Hyperledger fabric Go SDK](https://github.com/hyperledger/fabric-sdk-go)
- [Hyperledger fabric REST SDK](https://github.com/hyperledger/fabric-sdk-rest)

### `Note`

Hyperledger fabric also offers CA - Certificate of Authoriry for the network to manage and configure identity on your blockchain network
[Hyperledger fabrc CA service](http://hyperledger-fabric-ca.readthedocs.io/en/latest)

-------

@Jaz-3-0
