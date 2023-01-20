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

## dos-game

**dos-game**，一些经典游戏怀旧

## heimdall

**heimdall** 是一个导航首页的服务，nas/vps 上的服务多了，可以配置一个首页，方便使用。

个人默认导出非 80 端口，通过 nginx 在 80/443 端口反代

## komga

**komga** 是一个网页看 pdf 的工具，个人主要用这个看漫画。

## nas-tools

**nas tools** 是 NAS 媒体库资源归集、整理自动化工具，搭配了 **emby（媒体播放）** 和 **qBittorrent（bt 下载）**。

nas tools，设置参考 [nas tool 官方库](https://github.com/jxxghp/nas-tools/wiki)。

emby，我选择关闭服务器解码功能，由客户端进行解码，减轻服务端压力。emby 的服务端解码功能在每个用户的用户设置里关闭。

qBittorrent，默认的账号 admin，密码 adminadmin。

## nginx

**nginx** 个人使用 nginx 反代不同服务，使用局域网域名（SmartDns），不用记忆各种端口。

## rsshub

**rsshub**，帮助将一些服务转为 rss 订阅，具体使用见[rss 官网](https://docs.rsshub.app/)。

## SmartDns

[SmartDns 官方](https://github.com/pymumu/smartdns)
[Sukka 的文章：我有特别的 DNS 配置和使用技巧](https://blog.skk.moe/post/i-have-my-unique-dns-setup/)

**SmartDns**，这个没有用 docker 安装，直接使用 apt、yun 等安装即可。
这里只说两点用处，第一个是屏蔽广告，第二个是本地域名解析；需要分流的自行研究。
如果只需要屏蔽广告，可以考虑 AdGuard。

屏蔽广告策略 [anti-ad](https://anti-ad.net/anti-ad-for-smartdns.conf)。
