---
id: 10093
title: 转 WP改机型升级必备 Win10手机版Interop Tools详细使用教程
date: 2018-02-24T22:42:52+08:00
author: yangyx91
layout: post
guid: https://axiangwp.azurewebsites.net/?p=10093
permalink: /wp-win10-mobile-interop-tools.html
views:
  - "19068"
smilie_vote_4:
  - "2"
smilie_vote_2:
  - "7"
  - "7"
love:
  - "9"
smilie_vote_1:
  - "4"
smilie_vote_5:
  - "4"
smilie_vote_3:
  - "1"
smilie_vote_6:
  - "2"
categories:
  - Win10手机
---
步入2018年后，微软手机系统Win10 Mobile继续进入每月维护阶段，新系统也限制到少数Lumia机型升级。如果普通Lumia需要跨版本号升级，还得依赖注册表，修改WP机型来实现。所幸的是，XDA开发者社区推出了WP手机设备的越狱工具Interop Tools。

Interop Tools是一款新的适用于 Win10 Mobile/Win10 PC 等平台的手机越狱工具（无需电脑部署安装），安装流程:

**下载interop tools（preview）**：<a href="http://uwp.cn/app/https://www.microsoft.com/zh-cn/store/p/interop-tools-preview/9ntgwlc0d3cs?rtc=1" target="_blank" rel="noopener ”nofollow”" rel="nofollow" >查看Windows 10在线商店</a>

备用下载：<a href="http://pan.baidu.com/share/link?shareid=3655205665&uk=2740713692" target="_blank" rel="noopener" rel="nofollow" >百度网盘（包含组件扩展）</a>

如果是首次安装Interop Tools建议先安装组件。<a href="https://pan.baidu.com/wap/link?&shareid=2016289504&uk=2740713692" target="_blank" rel="noopener" rel="nofollow" >组件下载</a>（共有三个，请按顺序安装，每点击安装一个组件，需要稍等10至20秒后才点击安装下一个，因为系统也需要缓缓啊！）  
为了让interop tools商店版能够使用，请下载扩展应用。<a href="https://pan.baidu.com/wap/link?&shareid=1167646933&uk=2740713692" target="_blank" rel="noopener" rel="nofollow" >扩展下载</a>

如果你使用直接下载安装包的方式来进行安装，请先打开开发者模式（设置→更新及安全→面向开发人员→开发人员模式）再点击文件选择安装。应用程序大约1分钟左右就可以在程序列表中看到，如果没有，可能是由于你的设备中没有符合interop tools的组件，请先下载所需的组件。

具体使用**interop tools（preview）**:

启动**interop tools（preview）**，使用registry editor（注册表编辑器）/registry browser（注册表浏览器）：

注册表区域主要包括四个部分，数值类型（registry value type），地址（registry key path），键值（registry value name）以及数值（registry value date）。

现在进行注册表修改方法举例（以下默认registry value hive（注册表根值）为HKLM，HKLM为HKEY\_LOCAL\_MACHINE的缩写）：

**修改机型：**  
注册表地址：HKEY\_LOCAL\_MACHINE\SYSTEM\Platform\DeviceTargetingInfo  
键值（请分别输入）：PhoneModelName和phonemanufacturermodelname  
数值：

（例如RM-1010，你可以在设置 >系统>关于 中找到手机型号）  
（例如RM-1010_1000，你可以在 设置>附加程序>附加功能与信息 中的mauefacturer name（制造商名称）找到）  
Lumia650：RM-1154，RM-1154_15729  
Lumia640（已不支持秋季更新正式版）：RM-1113，RM-1113_1003  
Lumia640XL（已不支持秋季更新正式版）：RM-1096，RM-1096_1002  
Lumia950：RM-1118，RM-1118_11280  
Lumia950XL：RM-1116，RM-1116_11258

**修改区域版本：**  
地址：HKEY\_LOCAL\_MACHINE\SYSTEM\Platform\DeviceTargetingInfo  
键值：phonemobileoperatorname  
数值：  
000-CN→国行  
000-HK→港行

**非国行机器安装来电归属与骚扰电话识别：**  
地址：  
HKLM\Software\Microsoft\CallAndMessagingEnhancement\BlockingApp  
和HKLM\Software\Microsoft\CallAndMessagingEnhancement\CallOriginApp  
键值：  
ActiveBlockingAppUsermodelId和ActiveCallOriginAppUserModelId  
数值：  
这两个都修改为:Microsoft.BlockandFilter_8wekyb3d8bbwe!x571a03cey8c00y4028y9bc0y34dc30a5ac66x  
然后进电话,找到拦截的设置进去,点上最下边一个选项,然后进电话应用设置,就可以选择了。