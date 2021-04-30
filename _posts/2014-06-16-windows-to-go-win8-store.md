---
id: 4817
title: 娱乐、工作兼得，如何开启Windows To Go版Win8/Win8.1应用商店
date: 2014-06-16T15:05:04+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=4817
permalink: /windows-to-go-win8-store.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "5705"
baidu_record:
  - "1"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:4816;s:11:"_thumb_type";s:10:"attachment";}'
categories:
  - Win10
  - Win8.1
  - 未分类
---
刚刚，阿象介绍了<a href="http://www.axiangblog.com/windows-to-go-win8-1.html" target="_blank" rel="nofollow" >Win8.1也能随身带，如何打造Windows To Go版Win8.1 U盘系统</a>，成功将Win8、Win8.1系统安装至大容量U盘、移动硬盘，真正实现移动版Win8.1系统体验。 

这也意味着用户可以在任何一台支持USB接口的公共电脑、平板电脑设备上直接启动运行U盘版Win8.1系统，单独享用个人专属系统，包括桌面、收藏夹、个人数据等资料。 

当然，Windows To Go功能不仅可以打造移动U盘系统，同时也可以取代传统PE系统工具，直接参与到系统维护、修复计算机、数据备份还原等领域。 

不少用户安装完Windows To Go版Win8/Win8.1后，发现无法正常打开微软应用商店，这是怎么回事呢？如何才能开启呢？ 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1505_Wi1.jpg) 

其中，微软默认禁用Windows To Go版Win8应用商店功能，具体可以使用组策略开启；后来，微软默认开启Windows To Go版Win8.1应用商店，如果你遇到无法打开商店，请将屏幕分辨率手动调节至1024&#215;768及以上。 

下面，阿象还是带Win8用户如何开启Windows To Go版Win8应用商店，具体以Win8企业版为例，操作如下： 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1505_Wi2.jpg) 

1、使用组合键Win+R，打开运行； 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1505_Wi3.jpg) 

2、输入gpedit.msc，打开本地组策略编辑器； 

3、依次定位到：**计算机配置》管理模版》Windows组件**，打开右侧的&#8221;应用商店&#8221;； 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1505_Wi4.jpg) 

4、双击&#8221;允许应用上带在Windows To Go工作去上安装应用&#8221;，设置为&#8221;已启用&#8221;，确认即可生效； 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1505_Wi5.jpg) 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/061614_1505_Wi6.jpg) 

5、最后重启当前的Windows To Go版Win8系统，即可正常使用Win8应用商店，下载游戏或者应用。