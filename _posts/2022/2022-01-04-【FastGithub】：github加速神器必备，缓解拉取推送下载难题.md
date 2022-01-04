---
title: "【FastGithub】：github加速神器必备，缓解拉取/推送/下载难题"
subheading: hello world!
date: 2022-01-04 21:13:27 +08:00
author: 象叔叔
layout: post
permalink: /fastgithub-dotnet-tool.html
categories:
- 云开发
tags:  云开发
---

日前，楼主在国内dotnetcore社区刷到了这款万能神器【FastGithub】，一下子缓解了楼主这类小伙伴常头疼难题，可谓github加速神器，有效解决了github打不开、用户头像无法加载、releases无法上传下载、git-clone、git-pull、git-push失败等问题，可谓是居家常备酷软，现在一起来试试吧。

![图片](https://mmbiz.qpic.cn/mmbiz_png/9GCBOx7tR284scuUlYJ6LiapvAuuR06JjV2daGPkb3NEOfIR9oqf47QZ8iaN2YOeYu6A6u2U7119IaEVwCaYlX7Q/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")


**1 程序下载**：github-release

[https://github.com/dotnetcore/FastGithub/releases](https://github.com/dotnetcore/FastGithub/releases "https://github.com/dotnetcore/FastGithub/releases")

**2 部署方式**
2.1 windows-x64桌面：双击运行FastGithub.UI.exe

![图片](https://mmbiz.qpic.cn/mmbiz_png/9GCBOx7tR284scuUlYJ6LiapvAuuR06Jj26AU2ZPosaWkLJbcMxlibUXjsdcIevalIuRxb0mlB9hNWQ0hicjYzlsg/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")


2.2 windows-x64服务
    fastgithub.exe start // 以windows服务安装并启动
    fastgithub.exe stop // 以windows服务卸载并删除

2.3 linux-x64终端
    sudo ./fastgithub
    设置系统自动代理为http://127.0.0.1:38457，或手动代理http/https为127.0.0.1:38457

2.4 linux-x64服务
    sudo ./fastgithub start // 以systemd服务安装并启动
    sudo ./fastgithub stop // 以systemd服务卸载并删除
    设置系统自动代理为http://127.0.0.1:38457，或手动代理http/https为127.0.0.1:38457

2.5 macOS-x64：双击运行fastgithub
    安装cacert/fastgithub.cer并设置信任
    设置系统自动代理为http://127.0.0.1:38457，或手动代理http/https为127.0.0.1:38457
    具体配置详情

3 软件功能

    提供域名的纯净IP解析；
    提供IP测速并选择最快的IP；
    提供域名的tls连接自定义配置；
    google的CDN资源替换，解决大量国外网站无法加载js和css的问题；

4 证书验证


4.1 git

git操作提示SSL certificate problem
需要关闭git的证书验证：git config --global http.sslverify false


4.2 firefox

firefox提示连接有潜在的安全问题
设置->隐私与安全->证书->查看证书->证书颁发机构，导入cacert/fastgithub.cer，勾选“信任由此证书颁发机构来标识网站”

![图片](https://mmbiz.qpic.cn/mmbiz_png/9GCBOx7tR284scuUlYJ6LiapvAuuR06JjqKeUlsrjDn62gCjqHJHQryfoA1Od9NsRTHL0EMWf861w8sR7qicuKibg/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

5 安全性说明

FastGithub为每台不同的主机生成自颁发CA证书，保存在cacert文件夹下。客户端设备需要安装和无条件信任自颁发的CA证书，请不要将证书私钥泄露给他人，以免造成损失。

现在直奔主题，原版本分支
[https://github.com/dotnetcore/FastGithub/releases](https://github.com/dotnetcore/FastGithub/releases "https://github.com/dotnetcore/FastGithub/releases")

备用网盘：[https://pan.xunlei.com/s/VMs_7SebzHCtKdxJ1Mwh3iTPA1](https://pan.xunlei.com/s/VMs_7SebzHCtKdxJ1Mwh3iTPA1 "https://pan.xunlei.com/s/VMs_7SebzHCtKdxJ1Mwh3iTPA1")
提取码：b6gv

【[阅读原文](https://mp.weixin.qq.com/s?__biz=MzI4MzA2OTg1Ng==&mid=2247486946&idx=2&sn=8ddf1d0952237dd4bd9c6495df26825c&chksm=eb91112ddce6983b0caf59eb298e1eb5ef530fc3e787c68e67ddbea1a15d2b6a526ef0989551&token=2085422152&lang=zh_CN#rd "阅读原文")】


