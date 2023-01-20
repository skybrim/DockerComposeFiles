# Awesome Server

一些自建服务方案的整理

## 前置

debian/ubuntu 一键安装 docker 和 docker-compose

```shell
curl https://raw.githubusercontent.com/skybrim/ShellScript/master/debian_docker_install.sh | sh
```

docker-compose 常用命令

```
# 启动
docker-compose up -d
# 停止
docker-compose down
```

## nas-tools

**nas tools** 是 NAS 媒体库资源归集、整理自动化工具，搭配了 **emby（媒体播放）** 和 **qBittorrent（bt 下载）**。

nas tools，设置参考 nas tool [官方库](https://github.com/jxxghp/nas-tools/wiki)。

emby，我选择关闭服务器解码功能，由客户端进行解码，减轻服务端压力。emby 的服务端解码功能在每个用户的用户设置里关闭。

qBittorrent，默认的账号 admin，密码 adminadmin。
