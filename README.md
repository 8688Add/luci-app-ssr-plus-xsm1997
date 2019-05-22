# 不可描述的项目
本项目为基于coolsnowwolf的lede项目中的软件包开发，加入了kumasocks的支持的自用项目。可能存在bug，可能会不稳定。本项目会不定期地同步主线。

原repo：https://github.com/coolsnowwolf/lede

请一同把openwrt-kumasocks加入OpenWRT中编译。项目地址：https://github.com/xsm1997/openwrt-kumasocks

关于kumasocks：kumasocks为一个轻量级的透明代理转SOCKS5的网络工具，支持iptables redirect转发至SOCKS5代理。请在内网环境中使用。(https://github.com/xsm1997/KumaSocks)

注意：本项目基于coolsnowwolf的lede项目中的软件包开发，仅加入了kumasocks的支持。controller中的代码为经过编译的luac代码，未作改动。



This repo is based on the package of lede repo of coolsnowwolf, and I add the support of kumasocks. This repo is my self-use project. It could have bugs, and I don't promise the stability. This repo will be synchonized with upstream aperiodically.

Repo based on: https://github.com/coolsnowwolf/lede

Please place openwrt-kumasocks into the OpenWRT root. Repo link: https://github.com/xsm1997/openwrt-kumasocks

About kumasocks: kumasocks is a light-weighted transparent proxy to SOCKS5 converter network utility. It supports redirecting "iptables redirect" to SOCKS5 proxy. In China, please use it in local area network.

Be attention: This repo is based on the package of lede repo of coolsnowwolf, and I only add the support of kumasocks. The codes in controller are compiled luac codes, without modifing.
