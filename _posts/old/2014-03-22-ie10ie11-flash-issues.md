---
id: 4045
title: IE10/IE11无法显示Flash问题修复方案
date: 2014-03-22T16:07:20+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=4045
permalink: /ie10ie11-flash-issues.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
category_icon:
  - "4247"
post_icon:
  - "4296"
views:
  - "34918"
baidu_record:
  - "1"
bigfa_ding:
  - "2"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:5456;s:11:"_thumb_type";s:10:"attachment";}'
smilie_vote_1:
  - "6"
smilie_vote_6:
  - "1"
smilie_vote_5:
  - "5"
categories:
  - Win8.1
  - 未分类
---
IE11 Flash问题是不少Win8、Win8.1普通用户常遇到的麻烦事。从Win8开始，微软默认为IE浏览器集成Adobe Flash Player插件。之所以导致IE10/IE11 Flash问题，大多数来自IE浏览器安全权限以及系统问题。

这次，笔者也整理Adobe官方修复IE10/IE11无法显示Flash问题方案（<a href="http://helpx.adobe.com/flash-player/kb/flash-player-issues-windows-8.html" target="_blank" rel="nofollow" >详情访问这里</a>）

<a href="http://www.axiangblog.com/wp-content/uploads/2014/03/ie11-flash-issues1.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5448" src="http://www.axiangblog.com/wp-content/uploads/2014/03/ie11-flash-issues1.jpg" alt="ie11-flash-issues1" width="400" height="336" /></a>

解决方案一、关闭IE10/IE11的**Active刷选**功能

由于Adobe Flash Player IE版采用ActiveX控件加载方式运作，当IE10/IE11启用**Active刷选**功能后，Flash播放器将无法正常工作，另外，IE地址栏右侧也会显示一个蓝色禁止标识。

<a href="http://www.axiangblog.com/wp-content/uploads/2014/03/ie11-flash-issues2.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5449" src="http://www.axiangblog.com/wp-content/uploads/2014/03/ie11-flash-issues2.jpg" alt="ie11-flash-issues2" width="400" height="245" /></a>

这时，只需选择关闭**Active刷选**，即可恢复IE11的Flash播放器功能。

<a href="http://www.axiangblog.com/wp-content/uploads/2014/03/ie11-flash-issues2.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5449" src="http://www.axiangblog.com/wp-content/uploads/2014/03/ie11-flash-issues2.jpg" alt="ie11-flash-issues2" width="400" height="245" /></a>

解决方案二、启用IE10/IE11 **Flash Player加载项**

有时候，普通用户因为设置不当，禁用IE10/IE11 Flash Player加载项，导致类似Flash网页无法显示问题。这时，只需重新启用Flash加载项

具体操作如下：

1、打开IE10/IE11右上角设置功能，选择**管理加载项**下的**工具栏和扩展**

<a href="http://www.axiangblog.com/wp-content/uploads/2014/03/ie11-flash-issues4.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5451" src="http://www.axiangblog.com/wp-content/uploads/2014/03/ie11-flash-issues4.jpg" alt="ie11-flash-issues4" width="450" height="303" /></a>

2、启用Flash ActiveX空间功能

解决方案三、降低IE10/IE11区域安全级别

微软为IE10/IE11分别设置三类安全级别：**中、中-高、高**，当**区域安全级别**设置**高**时，Flash将无法加载播放。

<a href="http://www.axiangblog.com/wp-content/uploads/2014/03/ie11-flash-issues5.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5452" src="http://www.axiangblog.com/wp-content/uploads/2014/03/ie11-flash-issues5.jpg" alt="ie11-flash-issues5" width="450" height="326" /></a>

这时，我们可以将IE10/IE11浏览器的**Internt选项“**安全”页面下的**区域安全级别**调至默认（**中-高**）级别。

<a href="http://www.axiangblog.com/wp-content/uploads/2014/03/ie11-flash-issues6.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5453" src="http://www.axiangblog.com/wp-content/uploads/2014/03/ie11-flash-issues6.jpg" alt="ie11-flash-issues6" width="450" height="280" /></a>

解决方案四、重新安装IE版Flash插件

微软每个月的补丁日都会提供最新版Adobe Flash Player For IE版安全更新，普通用户可以开启Windows Udate获取更新或者手动下载离线安装包。

<a href="http://www.axiangblog.com/wp-content/uploads/2014/03/ie11-flash-issues7.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5454" src="http://www.axiangblog.com/wp-content/uploads/2014/03/ie11-flash-issues7.jpg" alt="ie11-flash-issues7" width="430" height="262" /></a>

除此之外，用户可以参考：**控制面板\系统和安全\Windows 更新\查看更新历史记录**，查询当前Flash更新信息。

<a href="http://www.axiangblog.com/wp-content/uploads/2014/03/ie11-flash-issues8.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5456" src="http://www.axiangblog.com/wp-content/uploads/2014/03/ie11-flash-issues8.jpg" alt="ie11-flash-issues8" width="450" height="347" /></a>

Adobe Flash Player For Win8/Win8.1版IE版下载：<a href="http://helpx.adobe.com/flash-player/kb/flash-player-issues-windows-8.html" target="_blank" rel="nofollow" >点击这里</a>