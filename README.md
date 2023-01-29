# Awesome Server

当你拥有一台服务器可以用来做什么？

## 目录

### 网络类

- [SmartDNS](#smartdns)
- [Nginx](#nginx)

### 工具类

- [导航页](#heimdall)
- [网页看 PDF(漫画)](#komga)
- [本地影音库](#nas-tools)
- [RSS 订阅](#rss)

### 游戏娱乐

- [dos-game](#dos-game)

## 安装 docker

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

## SmartDns

**SmartDns**，这个没有用 docker 安装，直接使用 apt、yun 等安装即可。

用途：

- 屏蔽广告（加载 anti-ad）
- 本地域名解析 （示例：address/www.example.com/1.2.3.4）
- 分流 （国内域名使用国内 dns）

[SmartDns 官方文档](https://github.com/pymumu/smartdns)

[Sukka：我有特别的 DNS 配置和使用技巧](https://blog.skk.moe/post/i-have-my-unique-dns-setup/)

[屏蔽广告策略 anti-ad](https://anti-ad.net/anti-ad-for-smartdns.conf)

## nginx

**nginx** 反代不同服务，使用局域网域名（SmartDns 解析），不用记忆各种服务的端口。

## heimdall

**heimdall** 是一个导航首页的服务，nas/vps 上的服务多了，可以配置一个首页，方便使用。

个人默认导出非 80 端口，通过 nginx 在 80/443 端口反代

## komga

**komga** 是一个网页看 pdf 的工具，个人主要用这个看漫画。

## nas-tools

**nas tools** 是 NAS 媒体库资源归集、整理自动化工具，搭配了 **emby（媒体播放）** 和 **qBittorrent（bt 下载）**。

**nas tools**，设置参考 [nas tools 官方仓库](https://github.com/jxxghp/nas-tools/wiki)。

**emby**，我选择关闭服务器解码功能，由客户端进行解码，减轻服务端压力，服务端解码功能在每个用户的用户设置里关闭。

**qBittorrent**，默认的账号 admin，密码 adminadmin。

## rss

使用的是 **rsshub** 搭配 **tiny tiny rss**。

**rsshub**，帮助将一些服务转为 rss 订阅，具体使用见[rss 官网](https://docs.rsshub.app/)。
由于服务搭建好是公开的，我的 docker 设置里加了一些对服务器资源使用的限制，防止被打爆。

**tiny tiny rss**，自建的集中拉取 rss 的服务，这个服务个人觉得挺耗费服务器性能的，加了资源使用的限制，配置低的慎用。
使用的是这位大佬的配置，请自行查看[文档](https://ttrss.henry.wang/zh)。

## dos-game

**dos-game**，一些 DOS 的经典游戏怀旧，可以直接网页运行，举例：《仙剑奇侠传 98 柔情版》
