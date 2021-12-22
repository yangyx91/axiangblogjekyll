---
title: 巧借阿里/腾讯【云函数】，定时刷新微信小程序AccessToken
date: 2021-03-27 21:13+08:00
author: 象叔叔
layout: post
permalink: /serverless-functions-wechat-accesstoken.html
categories:云函数
tags: 微信 云函数 云开发
---


接触过微信小程序开发业务的小伙伴，都会遇到需要获取AccessToken的业务场景，例如生成小程序码，消息推送，消息模板构造，这些都离不开AccessToken(全局唯一后台接口调用凭据)。目前，微信官方默认分配了2个小时的有效期，需我们定时刷新，避免凭据过期。之前，我们就折腾过阿里/腾讯【云函数】的定时任务，调度执行获取必应每日一图，同样，我们这次也能再次借助云函数，定时刷新微信小程序AccessToken，无人值守云端运行。

**官方介绍：**

https://developers.weixin.qq.com/miniprogram/dev/api-backend/open-api/access-token/auth.getAccessToken.html

**准备工具：**

uniCloud服务空间【可选阿里云、腾讯云】

小程序管理平台->开发->开发设置、获取appid、secret'

**操作步骤：**

1、新建一个云函数，其中请求URL：

https://api.weixin.qq.com/cgi-bin/token?grant_type=client_credential&appid=APPID&secret=APPSECRET

图片

2、上传部署云函数，开启定时任务，条件公式：【cron:0 0 * * * *】，即每天整点执行，即每天执行12次。这样的调度模式，能及时更新小程序的Token凭据

图片

3、设计云数据库，例如appid、appsecret、accesstoken、小程序名称、小程序类型，都可以存入数据表，定时更新accesstoken字段。

图片


**历史囤货**

[巧借api网关+云函数，一键获取微信小程序【openid】](http://mp.weixin.qq.com/s?__biz=MzI4MzA2OTg1Ng==&mid=2247486024&idx=3&sn=f5c083896bb85412b5daee9ef8c6224e&chksm=eb911687dce69f9165b2ae4217892aeee038c3e80ae1eb0d9814d3e1226ae18c8f06dafcd0a4&scene=21#wechat_redirect "巧借api网关+云函数，一键获取微信小程序【openid】")

[真香：【微信小程序】免费开通云开发/云数据库/云空间/云函数](http://mp.weixin.qq.com/s?__biz=MzI4MzA2OTg1Ng==&mid=2247485922&idx=4&sn=4b4f61cb246cb19d226395e2c3f3a5e7&chksm=eb91152ddce69c3b04a15d81ffbe623e16096d16895a066bcf918a9943fb57c572e3cb540cce&scene=21#wechat_redirect "真香：【微信小程序】免费开通云开发/云数据库/云空间/云函数")

[阿里/腾讯【云函数】真香：懒人版Node+定时搬运【必应每日一图】](http://mp.weixin.qq.com/s?__biz=MzI4MzA2OTg1Ng==&mid=2247485978&idx=2&sn=123b984607f02c9231475d66893b3abf&chksm=eb9116d5dce69fc32cb8eb50134627829f1155ec302121b4e57b74676365cdd8187f5f8ceff0&scene=21#wechat_redirect "阿里/腾讯【云函数】真香：懒人版Node+定时搬运【必应每日一图】")

