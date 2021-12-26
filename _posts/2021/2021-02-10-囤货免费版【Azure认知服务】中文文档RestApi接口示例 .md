---
title: "囤货：免费版【Azure认知服务】中文文档/RestApi接口示例 "
subheading: hello world!
date: 2021-02-10 21:13:27 +08:00
author: 象叔叔
layout: post
permalink: /azure-cognitive-service-free-restful-api.html
categories:
- 云开发
tags: Azure 云开发
---
之前，楼主分享过【Azure静态站点】/Azure Funtion搭建和使用操作，这次将继续带来更有趣的【Azure 认知服务】，借助Rest Api即可集成到之前的Azure静态站点，加入现在流行的计算机视觉，人脸识别，语音服务等功能。现在就来看下官方准备的中文文档和Rest Api接口示例吧。

![图片](https://mmbiz.qpic.cn/mmbiz_jpg/9GCBOx7tR2ibBBf1ZuMhrTpedFH9d8VsxWbF0nS7mlSpt4Asn2n52mia7JXzM3YnCJxYn0tlPn3y47WbzI3oBUdA/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

**Azure认知服务介绍：**

认知服务使每位开发人员无需具备机器学习的专业知识就能接触到 AI。只需要一个 API 调用，就可以将看、听、说、搜索、理解和加速决策的能力嵌入到应用中。利用新式应用程序开发让所有技能水平的开发人员都能轻松在其应用中添加 AI 功能。


**中文文档&Rest Api接口示例：**

![图片](https://mmbiz.qpic.cn/mmbiz_jpg/9GCBOx7tR2ibBBf1ZuMhrTpedFH9d8Vsxu80S54zP7h3rTOFDd8QAt3x2JLib0Jn82ib5s2pmZia6lGhKhibMfwQQFQ/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

官方接口使用上也非常简便，创建对应服务，获取授权key，即可开始使用不同区域的接口服务，比如香港节点。


**文本分析Text Analytics API (v3.0)**


中文文档：[https://docs.microsoft.com/zh-cn/azure/cognitive-services/text-analytics/](https://docs.microsoft.com/zh-cn/azure/cognitive-services/text-analytics/ "https://docs.microsoft.com/zh-cn/azure/cognitive-services/text-analytics/")

接口文档
[https://eastasia.dev.cognitive.microsoft.com/docs/services/TextAnalytics-v3-0/operations/Languages](https://eastasia.dev.cognitive.microsoft.com/docs/services/TextAnalytics-v3-0/operations/Languages "https://eastasia.dev.cognitive.microsoft.com/docs/services/TextAnalytics-v3-0/operations/Languages")



**计算机视觉 API Computer Vision API (v3.1)**


中文文档 

[https://docs.microsoft.com/zh-cn/azure/cognitive-services/computer-vision/](https://docs.microsoft.com/zh-cn/azure/cognitive-services/computer-vision/ "https://docs.microsoft.com/zh-cn/azure/cognitive-services/computer-vision/")


接口文档

[https://eastasia.dev.cognitive.microsoft.com/docs/services/computer-vision-v3-1-ga/operations/56f91f2e778daf14a499f21b](https://eastasia.dev.cognitive.microsoft.com/docs/services/computer-vision-v3-1-ga/operations/56f91f2e778daf14a499f21b "https://eastasia.dev.cognitive.microsoft.com/docs/services/computer-vision-v3-1-ga/operations/56f91f2e778daf14a499f21b")


![图片](https://mmbiz.qpic.cn/mmbiz_png/9GCBOx7tR2ibBBf1ZuMhrTpedFH9d8VsxJuhygY9hsBp6XMCm7Ujpym0dXZAyFgAJDX3oOb7vxUtwWs6bJXu9fA/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

实际使用：计算机视觉可以识别图片内容，很方便为一张图添加描述。


**面部识别 Face API - v1.0**

中文文档：

[https://docs.microsoft.com/zh-cn/azure/cognitive-services/face/apireference](https://docs.microsoft.com/zh-cn/azure/cognitive-services/face/apireference "https://docs.microsoft.com/zh-cn/azure/cognitive-services/face/apireference")


接口文档

[https://eastasia.dev.cognitive.microsoft.com/docs/services/563879b61984550e40cbbe8d/operations/563879b61984550f30395236](https://eastasia.dev.cognitive.microsoft.com/docs/services/563879b61984550e40cbbe8d/operations/563879b61984550f30395236 "https://eastasia.dev.cognitive.microsoft.com/docs/services/563879b61984550e40cbbe8d/operations/563879b61984550f30395236")

![图片](https://mmbiz.qpic.cn/mmbiz_png/9GCBOx7tR2ibBBf1ZuMhrTpedFH9d8Vsxu9e4AuTa9tzPlfU7hQWFGNe9kqoGfMJZPKkICJmx7wiah5Bl8s5KBYw/640?wx_fmt=png&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

实际使用：人脸识别可以区分性别、年龄、情绪、发型等不同特征


**表单识别器Form Recognizer API (v2.0)**


中文文档 

[https://docs.microsoft.com/zh-cn/azure/cognitive-services/form-recognizer/](https://docs.microsoft.com/zh-cn/azure/cognitive-services/form-recognizer/ "https://docs.microsoft.com/zh-cn/azure/cognitive-services/form-recognizer/")

接口文档 

[https://eastasia.dev.cognitive.microsoft.com/docs/services/form-recognizer-api-v2/operations/AnalyzeLayoutAsync](https://eastasia.dev.cognitive.microsoft.com/docs/services/form-recognizer-api-v2/operations/AnalyzeLayoutAsync "https://eastasia.dev.cognitive.microsoft.com/docs/services/form-recognizer-api-v2/operations/AnalyzeLayoutAsync")


**语音服务**

[https://docs.microsoft.com/zh-cn/azure/cognitive-services/speech-service/](https://docs.microsoft.com/zh-cn/azure/cognitive-services/speech-service/ "https://docs.microsoft.com/zh-cn/azure/cognitive-services/speech-service/")


![图片](https://mmbiz.qpic.cn/mmbiz_jpg/9GCBOx7tR2ibBBf1ZuMhrTpedFH9d8VsxRxzGoWy0DX33JrKxMeTt7elHWNxUG4tcMa273AdvygyrykOKGtbPug/640?wx_fmt=jpeg&tp=webp&wxfrom=5&wx_lazy=1&wx_co=1 "图片")

实际使用：目前中文语音神经网络正式版有 晓晓、云扬两款女声、男声，支持文本转语音、语音转文本，可应用到语音朗读等，提升了人机交互的友好性。


**历史囤货**

[【Azure静态Web应用】Blazor真香，原生跑Azure Function Api](/azure-static-web-free-blazor-function-api.html "【Azure静态Web应用】Blazor真香，原生跑Azure Function Api")

【[阅读原文](https://mp.weixin.qq.com/s?__biz=MzI4MzA2OTg1Ng==&mid=2247485840&idx=2&sn=a39154d1ece37bd6ddd296cf77cad8fd&scene=19#wechat_redirect "阅读原文")】
