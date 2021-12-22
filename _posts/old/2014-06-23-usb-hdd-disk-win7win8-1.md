---
id: 4964
title: 新手教程：如何U盘、硬盘安装Win7/Win8.1图文攻略
date: 2014-06-23T15:09:57+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=4964
permalink: /usb-hdd-disk-win7win8-1.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "15437"
baidu_record:
  - "1"
bigfa_ding:
  - "1"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:4963;s:11:"_thumb_type";s:10:"attachment";}'
smilie_vote_1:
  - "1"
smilie_vote_2:
  - "2"
smilie_vote_4:
  - "1"
categories:
  - Win10
  - Win8.1
  - 未分类
---
对于电脑新用户来说，第一门课就是学习如何全新安装Win7、Win8.1系统。在日常使用中，我们常常用到U盘安装、硬盘安装方式。前者一般适合全新机器，即不带系统的电脑；后者一般适用于已安装Windows的新老机器。 

这次，阿象也为Win7、Win8.1新用户整理了如何用U盘、硬盘安装Win7、Win8.1系统图文教程，具体参考如下： 

**一、U盘安装Win7、Win8.1篇  
** 

这也是市面上最欢迎的Windows安装方式，适合各类新老用户，无论裸机或者已安装Windows系统老机器。 

准备工具：Win7、Win8.1 MSDN ISO原版系统镜像（<a href="http://www.axiangblog.com/win8-1-resource-summary.html" target="_blank"  rel="nofollow" >点击下载</a>）、微软官方U盘制作工具**Windows 7 USB DVD Download Tool**（<a href="http://images2.store.microsoft.com/prod/clustera/framework/w7udt/1.0/en-us/Windows7-USB-DVD-tool.exe" target="_blank" rel="nofollow" >点击下载</a>、<a href="http://www.400gb.com/u/2574829/6532830" target="_blank"  rel="nofollow" >备份下载</a>，支持制作Win7、Win8、Win8.1、Server） 

测试环境：Win8.1全新环境 

1、下载安装微软U盘制作工具**Windows 7 USB DVD Download Tool；  
** 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062314_1509_UW1.jpg) 

2、如果你正在运行Win8、Win8.1，这时将提示&#8221;**下载安装.Net Framework 3.5**&#8220;组件，这时可以选择在线安装或者离线安装方式： 

A、在线安装： 

点击**下载并安装此功能**，即可自动联网，在线安装**.Net Framework 3.5；** 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062314_1509_UW2.jpg) 

B、离线安装： 

这时只需用虚拟光驱加载Win8/Win8.1 iso镜像，例如虚拟光驱盘符为X盘； 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062314_1509_UW3.jpg) 

然后使用Win+X组合键，打开&#8221;命令提示符：管理员&#8221;，输入以下代码： 

**dism.exe /online /enable-feature /featurename:NetFx3 /Source:X:\sources\sxs  
** 

//其中X代表当前虚拟光驱盘符 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062314_1509_UW4.jpg) 

3、继续安装微软U盘制作工具**Windows 7 USB DVD Download Tool**并运行主程序； 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062314_1509_UW5.jpg) 

4、点击Browse，浏览本地Win7、Win8、Win8.1 ISO系统镜像； 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062314_1509_UW6.jpg) 

5、点击下一步，选择USB device； 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062314_1509_UW7.jpg) 

6、接着切换选择目标U盘，最后点击Begin copying，即可开始制作U盘启动盘 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062314_1509_UW8.jpg) 

7、最后重启新电脑，切换BIOS引导顺序，即可开始使用U盘全新安装Win7、Win8.1系统。 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062314_1509_UW9.jpg) 

 

**二、硬盘安装Win7、Win8.1篇：  
** 

准备工具：Win7、Win8.1 MSDN ISO原版系统镜像（<a href="http://www.axiangblog.com/win8-1-resource-summary.html" target="_blank"  rel="nofollow" >点击下载</a>）、硬盘安装工具 nt6\_hdd\_installer_v3.1.4（<a href="http://www.400gb.com/u/2574829/6532830" target="_blank"  rel="nofollow" >点击下载</a>）。 

具体操作： 

1、使用WinRAR、7-zip解压缩工具直接解压Win7、Win8.1 ISO原版镜像到除C盘的任意盘根目录。 

注：一定不要解压到C盘，一定要解压到根目录。 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062314_1509_UW10.jpg) 

2，将nt6\_hdd\_installer主程序放在Windows安装目录，然后右击&#8221;以管理员身份运行&#8221;主程序； 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062314_1509_UW11.jpg) 

3、直接用鼠标点击第一项：【**1、安装** nt6 hdd installer】； 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062314_1509_UW12.jpg) 

4、这时nt6 hdd installer主程序将自动识别X盘根目录下Win7、Win8.1系统安装文件，最后选择【**2、重启】**； 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062314_1509_UW13.jpg) 

5、这时Windows将自动重启，手动选择重启选择nt6 hdd installer mode 1或者nt6 hdd installer mode 2即可自动进入Win7、Win8.1安装界面； 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062314_1509_UW14.jpg) 

6、最后输入Win7、Win8.1安装密钥、接受许可协议、自定义安装（格式化、分区或者合并），即可开始安装Windows系统。 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062314_1509_UW15.jpg) 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062314_1509_UW16.jpg) 

![](http://www.axiangblog.com/wp-content/uploads/2014/06/062314_1509_UW17.jpg)