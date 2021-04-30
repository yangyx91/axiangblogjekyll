---
id: 8190
title: Win10升级Win10 10586蓝屏PAGE FAULT IN NONPAGED AREA修复方案
date: 2015-11-11T02:53:58+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=8190
permalink: /win10-blue-screen.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "11442"
baidu_record:
  - "1"
smilie_vote_1:
  - "1"
categories:
  - Win10
  - 未分类
---
10月30日，微软为Windows爱好者推送了桌面版Win10 Build 10576预览版，宣布进入Win10 TH2开发渠道，系统稳定性和新功能更趋稳定，不过这次预览版推送让笔者的Win10电脑中枪，其中就有蓝屏报错“PAGE FAULT IN NONPAGED AREA”错误。

这个蓝屏错误并不陌生，网上部分Win7/Win8.1/Win10低版本升级Win10也会发生情况，官方论坛回应是第三方软件与系统的兼容问题，其中包括安全软件、程序冲突问题。

<!--more-->

<a href="http://www.axiangblog.com/wp-content/uploads/2015/11/win10-bluescreen01.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-8191" src="http://www.axiangblog.com/wp-content/uploads/2015/11/win10-bluescreen01.jpg" alt="win10-bluescreen01" width="450" height="281" /></a>  
具体症状如下：Win10升级流程完成后，重启后报错PAGE FAULT IN NONPAGED AREA，无法正常进入桌面，会自动重启，即使在安全模式下，也会重启蓝屏。

笔者实际测试后，Win10出现蓝屏报错后，会智能推荐玩家使用“重置此电脑”功能，这项功能可以帮助当前Win10恢复到旧版Win10 Build 10565平台，同时清除所有第三方程序和应用，最大程度减少第三方程序与Win10最新预览版之间的兼容冲突问题。

<a href="http://www.axiangblog.com/wp-content/uploads/2015/11/win10-bluescreen02.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-8192" src="http://www.axiangblog.com/wp-content/uploads/2015/11/win10-bluescreen02.jpg" alt="win10-bluescreen02" width="450" height="186" /></a>  
当然Win10重置功能无需插入U盘、DVD等安装介质，支持保留当前的设置和个人文件。

<a href="http://www.axiangblog.com/wp-content/uploads/2015/11/win10-bluescreen03.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-8193" src="http://www.axiangblog.com/wp-content/uploads/2015/11/win10-bluescreen03.jpg" alt="win10-bluescreen03" width="450" height="366" /></a>  
基本上重置Win10后，我们将回到旧版Win10 Build 10565平台，然后正常升级Win10 Build 10576/10586，即可。

补充：网友也发现关闭Win10的“快速启动”，也可以减少蓝屏报错概率。