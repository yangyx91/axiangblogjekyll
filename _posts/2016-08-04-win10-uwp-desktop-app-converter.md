---
id: 9533
title: Win10 RS1 UWP开发：微软Win32桌面应用Desktop App Converter转换器14393最新下载
date: 2016-08-04T22:16:36+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=9533
permalink: /win10-uwp-desktop-app-converter.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "8226"
baidu_record:
  - "1"
smilie_vote_2:
  - "1"
smilie_vote_4:
  - "2"
smilie_vote_1:
  - "1"
bigfa_ding:
  - "1"
categories:
  - Win10
  - Win10应用
  - 未分类
---
8月4日，微软在推送新一轮Win10 RS1红石正式版更新，同步也更新了“代号Centennial”的Windows桌面应用（Desktop App Converter）转换器工具，代号Project Centennial，支持Win10 14393及以后的平台开发。

借助Windows桌面应用（Desktop App Converter）转换器工具，传统Win32/.Net开发者可以将原先的桌面应用程序、游戏程序，转换编译为Win10 UWP应用，支持常见的msi、exe等桌面安装包格式，最终打包为Win10专属的appx程序包，可离线部署本地环境或上架Win10应用商店（预计7月份）。

<a href="http://www.axiangblog.com/win10-uwp-desktop-app-converter.html/win10-desktop-app" rel="attachment wp-att-9534" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9534" src="http://www.axiangblog.com/wp-content/uploads/2016/05/win10-desktop-app.jpg" alt="win10-desktop-app" width="450" height="234" /></a>

微软官方网站也上线了Win10 14393版本号的Desktop App Converter转换器工具，开发者允许将.NET 4.6.1或者Win32编译程序转换为UWP版，最终生成一个Appx程序包，可以以Add-AppXPackage PowerShell命令行进行本地开发环境部署安装。

这款Desktop App Converter转换器将在新版、独立的Windows环境下运行、转换各类Windows桌面安装包，在运行过程中将对安装包的注册表、文件系统I/O读写操作进行监视，最终生成AppX安装包，值得一试。

**Windows桌面应用Desktop App Converter转换器工具官网下载：3.3G**

文件名：Desktop App Converter &#8211; 0.1.15、Windows 10 Base Image &#8211; 10.0.14393.0

<a href="https://www.microsoft.com/en-us/download/details.aspx?id=53428" target="_blank"  rel="nofollow" >https://www.microsoft.com/en-us/download/details.aspx?id=53428</a>

支持64位Win10 Anniversary Update平台。

具体安装参考如下：

1、分别下载DesktopAppConverter.zip压缩包、BaseImage-14342.wim系统映像，比如下载路径为比如C:\Users\用户名\Downloads文件夹；

2、解压DesktopAppConverter.zip到当前本地文件夹，比如C:\Users\用户名\Downloads；

3、以管理员身份运行一个PowerShell命令窗口，输入：

**PS C:\> Set-ExecutionPolicy bypass**

4、继续运行以后命令，完成DesktopAppConverter安装任务：

**PS C:\Users\用户名\Downloads\DesktopAppConverter.ps1 -Setup -BaseImage .\BaseImage-14393.wim -Verbose**

5、最终重启，完成配置工作。

**参考MSDN文档，Desktop App Converter Preview (Project Centennial)上手教程**

<a href="https://msdn.microsoft.com/windows/uwp/porting/desktop-to-uwp-run-desktop-app-converter" target="_blank"  rel="nofollow" >https://msdn.microsoft.com/windows/uwp/porting/desktop-to-uwp-run-desktop-app-converter</a>