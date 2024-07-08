# Farcaster

Guide dev:

- https://docs.farcaster.xyz/hubble/hubble
- https://www.thehubble.xyz/intro/hubble.html

## Warpcast FID
You need to have a Warpcast account to do this, otherwise sign up here and it costs $5.
https://warpcast.com/~/invite-page/389634?id=23b86880

`Get FID:` Profile - > About

![warp](https://github.com/nodesynctop/Farcaster/assets/124766822/df6a2242-70d1-48e1-bc0f-7235dd441069)


## Minimum hardware requirement
4 Cores, 8G Ram,  400G SSD, Ubuntu 22.04

## Install Node

### 1. Server preparation
```
sudo apt update && apt upgrade -y
sudo apt install wget curl make clang net-tools pkg-config libssl-dev build-essential jq lz4 gcc unzip snapd -y
```
### 2. Install Docker
```
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
```
```
sudo curl -L "https://github.com/docker/compose/releases/download/v2.20.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
```

