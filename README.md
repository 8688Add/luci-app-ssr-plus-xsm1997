# luci-app-ssr-plus 修改版
### 中文
本项目为基于coolsnowwolf的lede项目中的软件包开发，加入了kumasocks的支持的自用项目。可能存在bug，可能会不稳定。本项目会不定期地同步主线。

原repo：https://github.com/coolsnowwolf/lede

请一同把openwrt-kumasocks加入OpenWRT中编译。项目地址：https://github.com/xsm1997/openwrt-kumasocks

关于kumasocks：kumasocks为一个轻量级的透明代理转SOCKS5的网络工具，支持iptables redirect转发至SOCKS5代理。请在内网环境中使用。(https://github.com/xsm1997/KumaSocks)

本项目和主线中的有如下不同之处：

+ 加入了kumasocks支持。
+ 默认屏蔽443端口的UDP连接（主要是QUIC协议），在开启UDP代理的情况下，对于Youtube App这类优先QUIC协议的应用，有明显的速度提升。
+ 加入了IPv6代理支持（仅TCP连接），需要让路由器工作在IPv6 NAT模式下。

### English

This repo is based on the package of lede repo of coolsnowwolf, and I add support of kumasocks. This repo is my self-use project. It could have bugs, and I don't promise the stability. This repo will be synchonized with upstream aperiodically.

Repo based on: https://github.com/coolsnowwolf/lede

Please place openwrt-kumasocks into the OpenWRT root. Repo link: https://github.com/xsm1997/openwrt-kumasocks

About kumasocks: kumasocks is a light-weighted transparent proxy to SOCKS5 converter network utility. It supports redirecting "iptables redirect" to SOCKS5 proxy. In China, please use it in local area network.

There are some differencies between this repo and upstream:

+ Add support of kumasocks.
+ Block UDP connection to 443 port by default (mainly QUIC protocol). When UDP proxy is enabled, it will bring remarkable speed-up to Apps like Youtube which prefer QUIC protocol. (In China only)
+ Add support of IPv6 proxy (only TCP). Your router need work on IPv6 NAT mode when using this feature.
