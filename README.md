<p align="center">
  <img height="100" height="auto" src="https://github.com/freshe4qa/farcaster/assets/85982863/1204cf4a-5320-4364-b954-9b8a78762ff9">
</p>

# Farcaster — Node

Official documentation:
>- [Guide](-)

Explorer:
>- [-](-)

### Minimum Hardware Requirements
 - 4x CPUs; the faster clock speed the better
 - 16GB RAM
 - 140GB of storage (SSD or NVME)
 - Ubuntu 20.04

Для установки нам нужно FID и RPC Ethereum Mainnet и Optimism Mainnet.

FID: Заходим на вкладку Profile, далее нажимаем на 3 точки, затем About. Там мы увидим FID.

RPC: Можем взять RPC через Chainlist или Alchemy.

Установка ноды:

```
sudo apt update && sudo apt upgrade -y
```

```
apt install curl iptables build-essential git wget jq make gcc nano tmux htop nvme-cli pkg-config libssl-dev libleveldb-dev tar clang bsdmainutils ncdu unzip libleveldb-dev -y
```
```
screen -S farcaster
```
```
curl -sSL https://download.thehubble.xyz/bootstrap.sh | bash
```
Здесь вставляем HTTPS RPC Ethereum Mainnet, далее Optimism Mainnet и FID.

После чего нода будет синхронизироваться, окно можно закрыть CTRL + A + D.

Отслеживать можно через графану - http://<ip сервера>:3000

Чтобы зайти обратно в логи: 
```
screen -r farcaster
```
