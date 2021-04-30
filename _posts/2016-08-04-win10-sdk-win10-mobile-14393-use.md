---
id: 9747
title: Win10 UWP开发：Win10 SDK、Win10 Mobile 14393仿真模拟器虚拟机安装、使用教程
date: 2016-08-04T22:28:57+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=9747
permalink: /win10-sdk-win10-mobile-14393-use.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "6269"
baidu_record:
  - "1"
smilie_vote_4:
  - "1"
love:
  - "1"
smilie_vote_1:
  - "1"
categories:
  - Web开发
  - Win10
  - Win10应用
  - Win10手机
  - 未分类
---
8月初，微软向全球Win10电脑、平板以及Xbox One平台推送了Win10一周年更新（Win10 Build 14393（1607）版本），带来诸多的功能和新特性。对于开发者朋友，微软也准备了Win10 SDK工具、开放UWP应用/游戏提交、Win10 mobile 14393模拟器等一系列便利，现在，Win10开发者、Win10爱好者可提前体验最新in10手机版的新特性，可以用于开发、学习等工作。

下面，笔者也分别为开发者、爱好者整理了Win10 SDK、Win10 Mobile 14393模拟器安装图文教程，各位朋友们一起来学习了解下。

<a href="http://www.axiangblog.com/win10-sdk-win10-mobile-14393-use.html/win10-rs-sdk-vs3" rel="attachment wp-att-9751" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9751" src="http://www.axiangblog.com/wp-content/uploads/2016/08/win10-rs-sdk-vs3.jpg" alt="win10-rs-sdk-vs3" width="450" height="317" /></a>注：Win10 Mobile模拟器默认需64位系统、Hyper-V虚拟技术服务，Win10家庭版用户可以参考“<a href="http://www.axiangblog.com/win10-home-pro-upgrade.html" target="_blank" rel="nofollow" ><strong>Win10家庭版升级Win10专业版图文实战教程</strong></a>”，开启Hyper-V服务，即可体验模拟器等服务。

<a href="http://7xn9ba.com1.z0.glb.clouddn.com/wp-content/uploads/2015/08/win10-mobile-vm01.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-7601" src="http://7xn9ba.com1.z0.glb.clouddn.com/wp-content/uploads/2015/08/win10-mobile-vm01.jpg" sizes="(max-width: 450px) 100vw, 450px" srcset="http://7xn9ba.com1.z0.glb.clouddn.com/wp-content/uploads/2015/08/win10-mobile-vm01.jpg 450w, http://7xn9ba.com1.z0.glb.clouddn.com/wp-content/uploads/2015/08/win10-mobile-vm01-300x183.jpg 300w" alt="win10-mobile-vm01" width="450" height="275" /></a>准备工具：

1、《<a href="http://www.axiangblog.com/win10-anniversary-sdk-win10-mobile.html" target="_blank"  rel="nofollow" >Win10一周年更新Win10 RS1 SDK、Win10 Mobile RS1 14393模拟器离线包官方下载</a>》，分别安装sdk、Win10 Mobile模拟器

2、《<a href="http://www.axiangblog.com/visual-studio-2015-update3.html" target="_blank"  rel="nofollow" ><strong>微软Visual Studio 2015 Update3官方免费下载</strong></a>》，选择自定义安装，即可勾选Win10 SDK、Win10 Mobile仿真模拟器，完成安装配置。

<a href="http://7xn9ba.com1.z0.glb.clouddn.com/wp-content/uploads/2015/08/win10-mobile-vm03.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-7602" src="http://7xn9ba.com1.z0.glb.clouddn.com/wp-content/uploads/2015/08/win10-mobile-vm03.jpg" sizes="(max-width: 450px) 100vw, 450px" srcset="http://7xn9ba.com1.z0.glb.clouddn.com/wp-content/uploads/2015/08/win10-mobile-vm03.jpg 450w, http://7xn9ba.com1.z0.glb.clouddn.com/wp-content/uploads/2015/08/win10-mobile-vm03-268x300.jpg 268w" alt="win10-mobile-vm03" width="450" height="503" /></a>3、打开VS 2015主程序，右侧窗口将提示是否更新“Universal Windows App development tools (version 1.4.1)”工具，按照提升，完成UWP开发工具的配置。

<a href="http://www.axiangblog.com/win10-sdk-win10-mobile-14393-use.html/win10-rs-sdk-vs" rel="attachment wp-att-9748" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9748" src="http://www.axiangblog.com/wp-content/uploads/2016/08/win10-rs-sdk-vs.jpg" alt="win10-rs-sdk-vs" width="400" height="268" /></a>4、现在在VS 2015新建一个项目，即可设定最低平台Win10 Mobile Build 10240、目标平台Win10 Mobile Build 14393模拟器.

<a href="http://www.axiangblog.com/win10-sdk-win10-mobile-14393-use.html/win10-rs-sdk-vs1" rel="attachment wp-att-9749" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9749" src="http://www.axiangblog.com/wp-content/uploads/2016/08/win10-rs-sdk-vs1.jpg" alt="win10-rs-sdk-vs1" width="500" height="182" /></a><a href="http://www.axiangblog.com/win10-sdk-win10-mobile-14393-use.html/win10-rs-sdk-vs2" rel="attachment wp-att-9750" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9750" src="http://www.axiangblog.com/wp-content/uploads/2016/08/win10-rs-sdk-vs2.jpg" alt="win10-rs-sdk-vs2" width="450" height="256" /></a>默认Win10 Mobile 14393仿真模拟器支持6种配置选项，可部署、安装应用/游戏。

**Win10开发教程《HTML5+JS》PDF下载**，<a href="http://pan.baidu.com/s/1dD9F2CT" target="_blank" rel="nofollow" >网盘下载</a>

支持Win8.1、Win10、Server 2012 R2等平台

范例教程：<a href="http://www.microsoftvirtualacademy.com/training-courses/developing-universal-windows-apps-with-c-and-xaml?OCID=WIP_r_Jan_Body_Academy_16" target="_blank" rel="nofollow" >开发第一个Win10 UWP应用</a>、<a href="https://developer.microsoft.com/zh-cn/windows/downloads/windows-10-developer-preview?OCID=insider" target="_blank" rel="nofollow" >安装Win10 SDK和Win10移动版仿真器的预览版</a>