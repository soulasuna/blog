---
title: "Config Mirror Source Of Ubuntu"
date: 2023-01-27T23:09:12+08:00
draft: false
---

# Set mirror source of Ubuntu
> For Ubuntu20.04

## Set mirror source

1. Backup sources.list file
```shell
cd /etc/apt/
sudo cp sources.list sources.list.bak
```
2. Edit sources.list file
```shell
sudo vi sources.list
```
> Mirror of USTC

```shell
deb https://mirrors.ustc.edu.cn/ubuntu/ focal main restricted universe multiverse
deb-src https://mirrors.ustc.edu.cn/ubuntu/ focal main restricted universe multiverse
deb https://mirrors.ustc.edu.cn/ubuntu/ focal-updates main restricted universe multiverse
deb-src https://mirrors.ustc.edu.cn/ubuntu/ focal-updates main restricted universe multiverse
deb https://mirrors.ustc.edu.cn/ubuntu/ focal-backports main restricted universe multiverse
deb-src https://mirrors.ustc.edu.cn/ubuntu/ focal-backports main restricted universe multiverse
deb https://mirrors.ustc.edu.cn/ubuntu/ focal-security main restricted universe multiverse
deb-src https://mirrors.ustc.edu.cn/ubuntu/ focal-security main restricted universe multiverse
deb https://mirrors.ustc.edu.cn/ubuntu/ focal-proposed main restricted universe multiverse
deb-src https://mirrors.ustc.edu.cn/ubuntu/ focal-proposed main restricted universe multiverse
```

3. Update mirror
```shell
sudo apt-get update
```

4. upgrade software
```shell
sudo apt-get upgrade
```
or
```shell
sudo apt-get dist-upgrade
```

**Note**: 
The difference between dist-upgrade and upgrade

1. dist-upgrade handles package dependencies flexibly
2. upgrade If there is a problem with the dependency package, upgrade will stop the update.


