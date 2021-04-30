---
id: 4041
title: Win8/Win8.1屏幕截图技巧：一键归零/自动保存桌面
date: 2014-03-22T15:48:07+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=4041
permalink: /win8-win8-1-winprintscreen.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
category_icon:
  - "4227"
post_icon:
  - "4226"
views:
  - "5677"
baidu_record:
  - "1"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:5497;s:11:"_thumb_type";s:10:"attachment";}'
categories:
  - Win8.1
  - 未分类
---
Windows下如何全屏截图？

对于普通用户来说，最常用方法就是使用PrintScreen键，借助**画图**完成全屏截图。如果你是Win8/Win8.1用户，直接使用Win+PrintScreen，自动将全屏截图保存在当前系统“屏幕截图”文件夹下。但是，很多用户希望实现一键归零、自动保存桌面。

**一、如何实现Win8/Win8.1屏幕截图“一键归零”？**（即截图名称从1开始计数）

操作如下：<a href="http://www.axiangblog.com/wp-content/uploads/2014/03/win8-1-winprintscreen1.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5492" src="http://www.axiangblog.com/wp-content/uploads/2014/03/win8-1-winprintscreen1.jpg" alt="win8-1-winprintscreen1" width="450" height="334" /></a>

1、右击开始按钮，打开运行窗口，或者使用Win+R组合键

<a href="http://www.axiangblog.com/wp-content/uploads/2014/03/win8-1-winprintscreen2.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5493" src="http://www.axiangblog.com/wp-content/uploads/2014/03/win8-1-winprintscreen2.jpg" alt="win8-1-winprintscreen2" width="420" height="281" /></a>

2、输入rgedit，打开注册表编辑器

3、依次定位至**HKEY\_CURRENT\_USER\Software\Microsoft\Windows\CurrentVersion\Explorer**

<a href="http://www.axiangblog.com/wp-content/uploads/2014/03/win8-1-winprintscreen3.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5494" src="http://www.axiangblog.com/wp-content/uploads/2014/03/win8-1-winprintscreen3.jpg" alt="win8-1-winprintscreen3" width="450" height="306" /></a>

4、选择**Explorer**，将右侧的ScreenshotIndex值改为1，重启生效。

<a href="http://www.axiangblog.com/wp-content/uploads/2014/03/win8-1-winprintscreen4.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5495" src="http://www.axiangblog.com/wp-content/uploads/2014/03/win8-1-winprintscreen4.jpg" alt="win8-1-winprintscreen4" width="450" height="311" /></a>

提醒：另外，我们也可以使用注册表导入功能，实现“一键归零”。注：该注册表支持重复使用。

<a href="http://www.axiangblog.com/wp-content/uploads/2014/03/win8-1-winprintscreen5.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5496" src="http://www.axiangblog.com/wp-content/uploads/2014/03/win8-1-winprintscreen5.jpg" alt="win8-1-winprintscreen5" width="450" height="232" /></a>

使用记事本，新建”**Win8屏幕截图.reg**“注册表文件，输入以下内容，保存生效。

Windows Registry Editor Version 5.00

[HKEY\_CURRENT\_USER\Software\Microsoft\Windows\CurrentVersion\Explorer]  
&#8220;ExplorerStartupTraceRecorded&#8221;=dword:00000001  
&#8220;ShellState&#8221;=hex:24,00,00,00,3d,28,00,00,00,00,00,00,00,00,00,00,00,00,00,00,\  
01,00,00,00,13,00,00,00,00,00,00,00,6a,00,00,00  
&#8220;UserSignedIn&#8221;=dword:00000001  
&#8220;SIDUpdatedOnLibraries&#8221;=dword:00000001  
&#8220;LastClockSize&#8221;=hex:2d,00,00,00,11,00,00,00,42,00,00,00,11,00,00,00,32,00,00,\  
00,11,00,00,00  
&#8220;GlobalAssocChangedCounter&#8221;=dword:00000051  
&#8220;AppReadinessLogonComplete&#8221;=dword:00000001  
&#8220;EnableAutoTray&#8221;=dword:00000000  
&#8220;ScreenshotIndex&#8221;=dword:00000001

<a href="http://www.axiangblog.com/wp-content/uploads/2014/03/win8-1-winprintscreen6.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5497" src="http://www.axiangblog.com/wp-content/uploads/2014/03/win8-1-winprintscreen6.jpg" alt="win8-1-winprintscreen6" width="450" height="120" /></a>

▲导入Win8屏幕截图.reg注册表

二、**如何实现Win8/Win8.1屏幕截图自动保存当前系统桌面？**

这时，我们需要借助Win8自带的**mklink**命令实现系统目录软链接，即将原**图片\屏幕截图**目录指定到**系统桌面**目录。

![](http://img.ithome.com/newsuploadfiles/2014/3/20140320_131000_353.JPG) 

▲全屏截图默认保存至Win8**图片**库**\屏幕截图**目录下

**操作如下：**

1、首先删除Win8/Win8.1系统内置**图片**库**\屏幕截图**文件夹

2、右击开始按钮，打开**命令提示符（管理员）**

![](http://img.ithome.com/newsuploadfiles/2014/3/20140320_131000_214.jpg) 

3、输入如下命令格式：

**mklink /j &#8220;C:\Users\当前用户名\Pictures\Screenshots&#8221; C:\Users\当前用户名\Desktop**

如当前Win8.1用户名为IT之家，即输入mklink /j &#8220;C:\Users\IT之家\Pictures\Screenshots&#8221; C:\Users\IT之家\Desktop

![](http://img.ithome.com/newsuploadfiles/2014/3/20140320_131000_967.JPG) 

4、这时，Win8/Win8.1系统默认**屏幕截图**重定向至**系统桌面**

![](http://img.ithome.com/newsuploadfiles/2014/3/20140320_131001_58.JPG) 

现在，我们使用Win+PrintScreen，就可以自动将全屏截图保存至当前桌面。

![](http://img.ithome.com/newsuploadfiles/2014/3/20140320_131001_326.JPG)