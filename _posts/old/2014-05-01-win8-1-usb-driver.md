---
id: 4437
title: 制作Win8.1安装U盘，如何保留原有数据？
date: 2014-05-01T14:07:41+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=4437
permalink: /win8-1-usb-driver.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "7170"
baidu_record:
  - "1"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:5105;s:11:"_thumb_type";s:10:"attachment";}'
categories:
  - Win10
  - Win8.1
  - 未分类
---
如何U盘安装Win8.1系统？对于普通用户来说，这已不是件难事，例如**U盘启动大师**，可以轻松帮你识别**MSDN原版系统**和**刻录U盘**，但美中不足的是，每次都是全盘格式化，无法保留U盘原有的数据。

对于8G、16G或32G大容量U盘用户来说，能否不格盘就可以制作Windows 8.1安装U盘吗？答案当然是肯定的。小编也为U盘“大用户们”精心整理了图文教程，不格盘也可以制作Win8.1安装U盘。

这次，我们请来微软自家U盘启动制作工具（**Windows 7 USB DVD Download tool**），支持制作Windows7及以上的系统。虽然微软自家工具默认自动抹除U盘所有数据，格盘刻录系统，但我们可以启用一项隐藏注册表，开启**Windows 7 USB DVD Download tool**自动保留U盘原有数据功能。

<a href="http://www.axiangblog.com/wp-content/uploads/2014/05/win8-1-usb-driver1.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5099" src="http://www.axiangblog.com/wp-content/uploads/2014/05/win8-1-usb-driver1.jpg" alt="win8-1-usb-driver1" width="450" height="239" /></a>

**长话不多说，具体操作步骤如下——**

1、下载安装<a href="http://images2.store.microsoft.com/prod/clustera/framework/w7udt/1.0/en-us/Windows7-USB-DVD-tool.exe" target="_blank" rel="nofollow" >Windows 7 USB DVD Download tool</a>工具；

2、打开记事本，新建空白文档，输入如下内容：

**Windows Registry Editor Version 5.00**

**//禁用 Windows 7 USB DVD Download tool U盘格式化功能**

**[HKEY\_CURRENT\_USER\Software\Microsoft\ISO Backup Tool]**

**&#8220;Version&#8221;=&#8221;1.0.30&#8221;**

**&#8220;Shortcut&#8221;=&#8221;1&#8221;**

**&#8220;DisableFormat&#8221;=dword:00000001**

**<a href="http://www.axiangblog.com/wp-content/uploads/2014/05/win8-1-usb-driver2.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5100" src="http://www.axiangblog.com/wp-content/uploads/2014/05/win8-1-usb-driver2.jpg" alt="win8-1-usb-driver2" width="442" height="246" /></a>  
** 

提醒：如果需要保留U盘数据，只需将最后一位改为1；格盘刻录时，只需该尾数改为0。

3、将以上的空白文档，另存为“**禁用Windows 7 USB DVD Download tool U盘格式化.reg**”注册表文件，注意将**文档txt后缀名更改为reg**格式；

4、运行导入该注册表文件；

<a href="http://www.axiangblog.com/wp-content/uploads/2014/05/win8-1-usb-driver3.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5101" src="http://www.axiangblog.com/wp-content/uploads/2014/05/win8-1-usb-driver3.jpg" alt="win8-1-usb-driver3" width="450" height="164" /></a>

5、现在我们就可以保留原有数据，制作Win8.1安装U盘，参考如下图文使用流程。

▼运行**Windows 7 USB DVD Download tool**，选择Browse，浏览Win8.1 with Update完整ISO系统镜像

<a href="http://www.axiangblog.com/wp-content/uploads/2014/05/win8-1-usb-driver4.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5102" src="http://www.axiangblog.com/wp-content/uploads/2014/05/win8-1-usb-driver4.jpg" alt="win8-1-usb-driver4" width="450" height="239" /></a>

▼选择USB模式，开始写入

<a href="http://www.axiangblog.com/wp-content/uploads/2014/05/win8-1-usb-driver5.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5103" src="http://www.axiangblog.com/wp-content/uploads/2014/05/win8-1-usb-driver5.jpg" alt="win8-1-usb-driver5" width="450" height="238" /></a>

▼工具默认提示数据风险（其实已开启保留U盘数据），选择Erase USB设备

<a href="http://www.axiangblog.com/wp-content/uploads/2014/05/win8-1-usb-driver6.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5104" src="http://www.axiangblog.com/wp-content/uploads/2014/05/win8-1-usb-driver6.jpg" alt="win8-1-usb-driver6" width="450" height="239" /></a>

▼正常将Win8.1 ISO镜像写入U盘

<a href="http://www.axiangblog.com/wp-content/uploads/2014/05/win8-1-usb-driver7.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5105" src="http://www.axiangblog.com/wp-content/uploads/2014/05/win8-1-usb-driver7.jpg" alt="win8-1-usb-driver7" width="450" height="244" /></a>

最后成功制作Win8.1安装U盘，同时也保留原有的U盘数据。看到这里，U盘大用户们，有没有心动？

如果你倾向抹除U盘，制作一个纯净版Win8.1安装U盘，可以关闭该注册表，使用**Windows 7 USB DVD Download tool**或者**U盘大师。**