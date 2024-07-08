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
`4 Cores, 16G Ram,  min 300G SSD, Ubuntu 22.04`

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
### 3. Config node

`3.1`. Warpcast FID , you get before

`3.2`. You need provide ETH and RPC on the OP mainnet network. You can get it from https://dashboard.alchemy.com/apps/
![Farcaster](https://github.com/nodesynctop/Farcaster/assets/124766822/90d51120-9ea0-49f9-ac96-d4657364549c)

`3.3`. Run and config

```
curl -sSL https://download.thehubble.xyz/bootstrap.sh | bash
```
![Farcaster1](https://github.com/nodesynctop/Farcaster/assets/124766822/9964f754-961e-44a5-b410-b2acaacc5291)

`3.4` Logs show

![Farcaster3](https://github.com/nodesynctop/Farcaster/assets/124766822/bbd414c2-8533-4f20-9df5-fc093a36dcc9)

`3.5`. You can check whether the FID is correct with the code below.

```
docker logs hubble-hubble-1 2>&1 | grep "Hub Operator FID"
```
`3.6` Check logs - sync
```
docker logs -f hubble-hubble-1
```




