---
id: 9262
title: Build2016：VS2015快速入门开发Xbox One开发版UWP应用
date: 2016-03-31T22:23:18+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=9262
permalink: /build2016-vs2015-xbox-one-uwp.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "3480"
baidu_record:
  - "1"
smilie_vote_1:
  - "1"
categories:
  - Web开发
  - Win10
  - Xbox游戏
  - 未分类
---
自3月30日起，Win10开发者可以为Xbox One主机/电视引入UWP通用应用和游戏，<a href="http://www.axiangblog.com/xbox-one-win10-dev-mod.html" target="_blank" rel="nofollow" >只需将国行/国际版Xbox One主机解锁开发者模式</a>后，即可用Visual Studio 2015 Update2开发工具搭建Xbox One版UWP应用，不容错过。

一、开发Xbox One版UWP应用准备工作：

<a href="http://www.axiangblog.com/build2016%ef%bc%9avs2015%e5%bf%ab%e9%80%9f%e5%85%a5%e9%97%a8%e5%bc%80%e5%8f%91xbox-one%e5%bc%80%e5%8f%91%e7%89%88uwp%e5%ba%94%e7%94%a8.html/xbox-uwp-vs1" rel="attachment wp-att-9263" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9263" src="http://www.axiangblog.com/wp-content/uploads/2016/03/xbox-uwp-vs1.jpg" alt="xbox-uwp-vs1" width="450" height="252" /></a>  
1、一个Windows开发中心账号，<a href="https://dev.windows.com/" target="_blank" rel="nofollow" >点击注册</a>；  
2、申请加入Windows预览会员项目，获取最新Win10 SDK开发预览版，<a href="https://insider.windows.com/" target="_blank" rel="nofollow" >点击注册</a>；  
3、最低64位Win10环境  
4、配置一台上网的Xbox One主机，推荐有线上网；  
5、Xbox One主机建议保留30G可用空间。

二、搭建开发平台的Win10 PC设备：

1、推荐<a href="http://www.axiangblog.com/visual-studio-2015-update2.html" target="_blank" rel="nofollow" >下载安装微软开发套件Visual Studio 2015 Update 2正式版</a>，确保安装了“Visual Studio通用Windows应用开发工具”开发组件；

2、安装Win10 SDK build 14295预览版开发套件，<a href="http://go.microsoft.com/fwlink/p/?LinkId=780552" target="_blank" rel="nofollow" >点击这里获取</a>。

三、配置Xbox One主机的开发模式，参考《<a href="http://www.axiangblog.com/xbox-one-win10-dev-mod.html" target="_blank" rel="nofollow" >国行/国际版Xbox One主机如何解锁开发者模式</a>》

四、以Visual Studio 2015创建HTML/Javascript编译UWP为范例；

1、打开Visual Studio 2015的项目，右击项目属性，配置Debugging活动页面，将调试器更改为“远程计算机”，输入Xbox One主机IP地址，例如192.168.2.101，身份验证更改为“通用（未加密协议）Unencrypted Protocol ”；

<a href="http://www.axiangblog.com/build2016%ef%bc%9avs2015%e5%bf%ab%e9%80%9f%e5%85%a5%e9%97%a8%e5%bc%80%e5%8f%91xbox-one%e5%bc%80%e5%8f%91%e7%89%88uwp%e5%ba%94%e7%94%a8.html/xbox-uwp-vs2" rel="attachment wp-att-9264" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9264" src="http://www.axiangblog.com/wp-content/uploads/2016/03/xbox-uwp-vs2.jpg" alt="xbox-uwp-vs2" width="450" height="220" /></a>  
2、按下F5或调试，即可在Xbox One主机上部署你的UWP应用；

3、首次部署时，Visual Studio 2015会提示开发者为Xbox One配置一个PIN安全码，（当你打开Xbox One主机的开发模式后将自动获取一个PIN），最终在Visual Studio套件中输入PIN，即可完成远程认证；

4、当PIN配对完成后，Xbox One版UWP应用将自动部署安装，需要等待很长的处理时间；

5、最后成功在Xbox One主机上运行第一个UWP应用，Hello world！

<a href="http://www.axiangblog.com/build2016%ef%bc%9avs2015%e5%bf%ab%e9%80%9f%e5%85%a5%e9%97%a8%e5%bc%80%e5%8f%91xbox-one%e5%bc%80%e5%8f%91%e7%89%88uwp%e5%ba%94%e7%94%a8.html/xbox-uwp-vs3" rel="attachment wp-att-9265" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9265" src="http://www.axiangblog.com/wp-content/uploads/2016/03/xbox-uwp-vs3.jpg" alt="xbox-uwp-vs3" width="450" height="253" /></a>  
参考微软开发者中心：<a href="https://developer.microsoft.com/zh-cn/windows/windows-apps/uwp-on-xbox" target="_blank" rel="nofollow" >Xbox One开发者预览版上的UWP应用</a>