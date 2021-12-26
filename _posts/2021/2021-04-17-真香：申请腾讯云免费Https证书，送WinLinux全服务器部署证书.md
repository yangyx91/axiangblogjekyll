---
title: "真香：申请腾讯云免费Https证书，送Win/Linux全服务器部署证书"
subheading: hello world!
date: 2021-04-17 21:13:27 +08:00
author: 象叔叔
layout: post
permalink: /tencent-cloud-free-ssl-https.html
categories:
- 云开发
tags: Https 云开发
---

对于折腾免费Https证书的童鞋来说，阿里云、腾讯云和各大云服务商都是首选。在这些平台上面，我们都可以申请一份TrustAsia颁发的DV SSL证书，有效期一年，非常便于在服务器上面部署Https证书。日前，楼主也在腾讯云上买了新域名，顺路了申请了免费SSL证书，令人惊喜的是，腾讯云颁发SSL证书时，会自动导出Win/Linux全服务器所需的部署证书，非常人性化，极大了简便了SSL证书文件格式的互转，懒人的福利+1。

![图片](https://mmbiz.qpic.cn/mmbiz_jpg/9GCBOx7tR29TenQ4ON766D5BBpx6XkQbIyeOKtczt4W4wWk76wSsph86uGmyFBKzCP7gd3MdhqAuKeT3FwTJPg/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

**申请流程：**

1、进入腾讯云后台，进入SSL证书，“申请免费证书”

![图片](https://mmbiz.qpic.cn/mmbiz_jpg/9GCBOx7tR29TenQ4ON766D5BBpx6XkQbT0TVYqRPX4vLUPj105epRaryxCicrTIpHIfYame3icsJvyoxspddcNRg/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

2、输入证书绑定域名，私钥

![图片](https://mmbiz.qpic.cn/mmbiz_jpg/9GCBOx7tR29TenQ4ON766D5BBpx6XkQbqOXA21iaagFrQqENr8O3poQ9ljqmfw6Um0E7BfzH8Wrricm5cEBJTNbg/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

3、再次对绑定域名验证，可选DNS验证、或者文件验证。楼主推荐DNS验证，只需添加一条TXT记录，即可快速验证。

![图片](https://mmbiz.qpic.cn/mmbiz_jpg/9GCBOx7tR29TenQ4ON766D5BBpx6XkQbUVJvh7NCvpScAZM80sNCXlqHOEHoY6k3H4CrJaM9Ny6qII7lqOGGuA/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

4、SSL证书申请通过后，点击下载，即可获取一份“全服务器部署证书”

![图片](https://mmbiz.qpic.cn/mmbiz_jpg/9GCBOx7tR29TenQ4ON766D5BBpx6XkQbnd1DD508zQQXTfJwX2He1S6C3ibFSqeT7B1ibpqHH5v0Ny5txaicT65uA/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

小贴士：这份全服务器部署证书，包含SSL原始的PEM+Key，也包含了市面上主流的Apache(Linux)、IIS(Windows Server)、Nginx(Linux)、Tomcat(Linux)服务器平台对应的证书文件格式，可谓是真香。

【[阅读原文](https://mp.weixin.qq.com/s?__biz=MzI4MzA2OTg1Ng==&mid=2247486148&idx=4&sn=3255bf937d8d5927650d7df9917f787a&scene=19#wechat_redirect "阅读原文")】
