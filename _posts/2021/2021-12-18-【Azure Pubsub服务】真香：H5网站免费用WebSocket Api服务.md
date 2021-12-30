---
title: "【Azure Pubsub服务】真香：H5网站免费用WebSocket Api服务"
subheading: hello world!
date: 2021-12-18 21:13:27 +08:00
author: 象叔叔
layout: post
permalink: /azure-web-pubsubs-websocket-free.html
categories:
- 云开发
tags: Azure 云开发
---

在最近一次微软Azure产品更新公告中，原先【Azure Web Pubsub服务】预览版正式转正，正式推出了一款免费版服务，方便小伙伴使用Websocket和发布-订阅模式，生成各种实时消息传递的H5网站/Web应用。借助这项实时功能，我们可以在服务器和客户端之间发布内容更新，不需要轮询最新更新，也不需要为更新提交新的 HTTP 请求，极大的给自己项目和业务减负，可谓真香。

![图片](https://mmbiz.qpic.cn/mmbiz_jpg/9GCBOx7tR2icWcibmPYhNuIMXy3xW2tKniaLCxfHCdiaMrkrbqx1X24IxvSnamfTozDyVNdb8WktxInJV3oDCQersA/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

**官方文档：**

[https://docs.microsoft.com/zh-cn/azure/azure-web-pubsub/overview](https://docs.microsoft.com/zh-cn/azure/azure-web-pubsub/overview "https://docs.microsoft.com/zh-cn/azure/azure-web-pubsub/overview")

目前，【Azure Pubsub服务】官方提供了丰富的教程案例，对应SDK支持了市面上主流开发语言，大家也能选择免费层，值得一试。

![图片](https://mmbiz.qpic.cn/mmbiz_jpg/9GCBOx7tR2icWcibmPYhNuIMXy3xW2tKniasNaYM0FrLspg4uysWXia2EqOXT3wmTFX3UQkvuniblove7DSicYuECSrw/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

![图片](https://mmbiz.qpic.cn/mmbiz_jpg/9GCBOx7tR2icWcibmPYhNuIMXy3xW2tKniaWsXlcFXr2cvlrUPejKvcmgDmOFhIiaWucRgZMnOu1IhJDQR6iaiaMCaKw/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

其中官方也推出了HTML5版websocket演示页面，交互和代码清晰，很容易上手。

参考：
[https://azure.github.io/azure-webpubsub/demos/clientpubsub.html](https://azure.github.io/azure-webpubsub/demos/clientpubsub.html "https://azure.github.io/azure-webpubsub/demos/clientpubsub.html")

![图片](https://mmbiz.qpic.cn/mmbiz_jpg/9GCBOx7tR2icWcibmPYhNuIMXy3xW2tKniahEAicibjTITSfHyZZJ38Zwn9AYoKI6v8YUjWia3cQvVo0VbWxcSNmCtAg/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

![图片](https://mmbiz.qpic.cn/mmbiz_jpg/9GCBOx7tR2icWcibmPYhNuIMXy3xW2tKniahxyXn3dlgAl7RQGyYa681qmfdib3ibkqOvWSxJYyfG8kiadAukibAe0Rzg/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

在浏览器F12开发者工具里，WS栏目，能看到每次websocket消息推送和接收，极大的减少了HTML5页面业务和复杂度。

![图片](https://mmbiz.qpic.cn/mmbiz_jpg/9GCBOx7tR2icWcibmPYhNuIMXy3xW2tKniaI84zOxLlCR8NR18IPZZGia1ssz7iaCJN1nLu4fxeYeTC2kwTaLV7Hujg/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

![图片](https://mmbiz.qpic.cn/mmbiz_jpg/9GCBOx7tR2icWcibmPYhNuIMXy3xW2tKnia8ibCtiaBC4J8mozdf9VB9GCAGuVS6QV1RNTAzBtDkx4DMN7Nu0fu6gcw/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

现在就来注册一份Azure Pubsub服务吧。

【[阅读原文](https://mp.weixin.qq.com/s?__biz=MzI4MzA2OTg1Ng==&mid=100003273&idx=4&sn=42cbd3f341369d7154edd3ba940f82e2&chksm=6b9111065ce698102a14954060e0b00a5c2702d8c31ed4c6c966e1345887b87a6f0ffa7f0d7d#rd "阅读原文")】