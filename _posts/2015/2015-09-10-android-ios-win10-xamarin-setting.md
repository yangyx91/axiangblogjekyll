---
id: 7744
title: 安卓/iOS/Win10跨平台方案Xamarin开发环境部署、安装教程
date: 2015-09-10T07:49:42+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=7744
permalink: /android-ios-win10-xamarin-setting.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
baidu_record:
  - "1"
views:
  - "8941"
smilie_vote_1:
  - "1"
love:
  - "1"
categories:
  - Asp.Net
  - Web开发
  - Win10
  - 未分类
---
提到国外C#跨平台开发解决方案，不得不提Xamarin，最早始创于2011年，现已覆盖安卓、苹果、Windows Phone、Win10等主流移动平台的应用、游戏开发服务，非常适合C#、.NET爱好者。

注：国内开发者也可以选择COCOS等开发方案。

由于国内特殊的网络环境，Xamarin无法在线获取更新，因此推荐手动部署Xamarin开发环境，下面笔者也分享下各类资源包的下载和安装。

开发工具：Win10、VS 2015、notepad++等

<a href="http://www.axiangblog.com/wp-content/uploads/2015/09/xamarin-setting.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-7746" src="http://www.axiangblog.com/wp-content/uploads/2015/09/xamarin-setting.jpg" alt="xamarin-setting" width="450" height="241" /></a>资源部署：

1、下载安装Java JDK v1.7.0，<a href="http://download.xamarin.com/Installer/MonoForAndroid/jdk-7u71-windows-i586.exe" target="_blank" rel="nofollow" >点击这里</a>，127MB

注：无论32位、64位Windows，都需要安装32位Java JDK。

2、下载安装Android SDK for Windows v22.0，<a href="http://dl.google.com/android/installer_r22-windows.exe" target="_blank" rel="nofollow" >点击这里</a>，83MB

注：这项组件可以完成主要SDK安装方案，部署各类相关的IDE控件。

3、配置Android SDK管理器工具，支持在GUI界面下部署以下组件：

Android SDK Tools  
Android SDK Platform-tools  
Android SDK Build-tools  
Android API 15  
Android API 19  
Android API 21

4、下载安装Android NDK for Windows r10d版本，注：暂无找到资源

5、下载配置GTK# v2.12.26，<a href="http://download.xamarin.com/GTKforWindows/Windows/gtk-sharp-2.12.26.msi" target="_blank" rel="nofollow" >点击这里</a>，24MB

6、下载配置Xamarin Studio v5.9.3扩展，<a href="http://download.xamarin.com/studio/Windows/XamarinStudio-5.9.3.1-0.msi" target="_blank" rel="nofollow" >点击这里</a>

<a href="http://www.axiangblog.com/wp-content/uploads/2015/09/xamarin-01.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-7747" src="http://www.axiangblog.com/wp-content/uploads/2015/09/xamarin-01.jpg" alt="xamarin-01" width="450" height="297" /></a>

7、最后下载配置Xamarin v3.11.590主程序，<a href="http://download.xamarin.com/studio/Windows/XamarinStudio-5.9.3.1-0.msi" target="_blank" rel="nofollow" >点击这里</a>，306MB

## <a href="http://www.axiangblog.com/win10-visual-studio-2015-rtm.html" data-slimstat-type="1" data-slimstat-callback="true" data-slimstat-tracking="false" target="_blank"  rel="nofollow" >相关资源：《Win10/安卓/iOS开发套件Visual Studio 2015正式版版官方下载》</a> {.article-title}

注：当完成以上所有组件安装配置后，开发者需重启Windows完成配置，确保各类组件正常运行。