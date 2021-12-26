---
title: "【Azure静态Web应用】Blazor真香，原生跑Azure Function Api"
subheading: hello world!
date: 2020-11-20 21:13:27 +08:00
author: 象叔叔
layout: post
permalink: /azure-static-web-free-blazor-function-api.html
categories:
- 云开发
tags: Azure 云开发
---
早前，楼主分享了【Azure静态Web应用】真香，免费囤货个人站点，现在【Azure静态Web应用】再次与时俱进，原生运行.Net5/6 Blazor PWA站点，充分发挥WebAssembly技术。日前，楼主再次查看微软文档、实地操作后，再次发现，主站点可原生部署Azure Function函数应用Api，许多后端数据可以走api和数据库层交互，实时渲染表现层。

![图片](https://mmbiz.qpic.cn/mmbiz_png/9GCBOx7tR2icAibNn3f2kb8ge94OA7uzIC3zc9P45yR4GzlXkCbQJf9GVq6FlFdwN1jMc7ESOfIrbKOoHibQUmgDA/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

通俗的说：在一个Azure Static Web Apps【Azure静态Web应用】，可以部署两个项目：一个Blazor主应用，另一个API（可选Azure Function函数应用），Azure工作流会自动同时部署两项目，路由也是走内部，非常简便。

![图片](https://mmbiz.qpic.cn/mmbiz_png/9GCBOx7tR2icAibNn3f2kb8ge94OA7uzICECJ8khNIDn6cRtd4tnic3WxQTuZez51V67QIkgQcM0pMou7ZRngOo0A/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

**【将API发布到Azure静态Web应用】操作演示教程：**

[https://docs.microsoft.com/zh-cn/learn/modules/publish-static-web-app-api-preview-url/](https://docs.microsoft.com/zh-cn/learn/modules/publish-static-web-app-api-preview-url/ "https://docs.microsoft.com/zh-cn/learn/modules/publish-static-web-app-api-preview-url/")

以往，纯前端和API交互是跨域请求，而【Azure静态Web应用】改变了这个现状，现在直接让Blazor PWA在同域下调用API，让API去获取数据操作。


![图片](https://mmbiz.qpic.cn/mmbiz_jpg/9GCBOx7tR2icAibNn3f2kb8ge94OA7uzICbSReU9tiahNXlFqZ1fm6OT9edWawVQBxKTGNKdd8R7ktqAich8joZzicA/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

比如在网页上按钮触发一个api，在浏览器F12网络请求，可以清楚的看到这个同域的api请求，无需分开端口号请求。

![图片](https://mmbiz.qpic.cn/mmbiz_png/9GCBOx7tR2icAibNn3f2kb8ge94OA7uzICHdUiaOM9G0HWV8sskefEy1pOJicQzbXBOnPHKcpWN6lvGOp8eRdJbL1A/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

感兴趣的小伙伴，也欢迎上车：[技巧：微软Azure原生升级.NET 5.0+Blazor PWA网页](https://mp.weixin.qq.com/s?__biz=MzI4MzA2OTg1Ng==&mid=2247485327&idx=3&sn=1bc0ddb5dd546b6986479bc2a87983ed&chksm=eb911b40dce692565606db57c9d985c563b13499d4ffe49879113c4de04b08ec9ceb5df9b57a&scene=21#wechat_redirect "技巧：微软Azure原生升级.NET 5.0+Blazor PWA网页")

【[阅读原文](https://mp.weixin.qq.com/s?__biz=MzI4MzA2OTg1Ng==&mid=2247485388&idx=1&sn=0b121904f6df76f076d94f3997b6ba10&chksm=eb911b03dce692151cd2edf44b9e95c1f3f5e081edc151c583aa96a320d63b372e48a4a008c0&scene=21#wechat_redirect "阅读原文")】
