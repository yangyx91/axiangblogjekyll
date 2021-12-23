---
id: 8168
title: 开发入门指南：什么是Win10通用应用（Universal Windows App）？
date: 2015-10-26T03:45:14+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=8168
permalink: /win10-universal-windows-app.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "4283"
baidu_record:
  - "1"
categories:
  - Web开发
  - Win10
  - 未分类
---
对于刚升级Win10童鞋，听到微软最多的宣传语，就是统一Win10生态圈，统一Win10通用应用UWP。那这个Win10通用应用解决方案到底是什么，有哪些优势？

通用Windows应用是一种基于通用Windows平台 (UWP) 构建的Windows体验，它首次作为Windows RT运行时在Win8中引入。用户希望其体验在所有设备上均为移动版，并且希望使用现有的最方便或最高效的设备完成任务，此理念是通用Windows应用的核心。

<!--more-->

<a href="http://www.axiangblog.com/wp-content/uploads/2015/10/win10-uwp-intro.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-8169" src="http://www.axiangblog.com/wp-content/uploads/2015/10/win10-uwp-intro.jpg" alt="win10-uwp-intro" width="450" height="115" /></a>  
通过Win10，你可以更加轻松地为UWP开发应用，并且只需一个API集、一个应用包和一个应用商店，即可访问所有Win10设备 – PC、平板电脑、手机等。对许多屏幕大小以及各种交互模型（无论是触控、鼠标和键盘、游戏控制器还是笔）的支持也更加轻松。

**那么，什么是 Universal Windows App？**

是什么使通用 Windows 应用不同寻常？以下特性使 Windows 10 上的通用 Windows 应用与众不同。

1、你的目标设备系列，而非某个操作系统。

设备系列可标识在其中的设备上所需的 API、系统特性和行为。它还可以确定在其上安装应用商店应用的设备集。

2、应用使用 .AppX 打包格式进行打包和分配。

所有通用Windows应用均可作为AppX程序包进行分配。这提供了值得信赖的安装机制，并确保应用无缝部署和更新。

3、存在一个适用于所有设备的应用商店。

注册为应用开发人员后，你可以向应用商店提交应用，并使其在所有设备系列或仅在所选设备系列上可用。你将在一个位置上提交和管理适用于 Windows 设备的所有应用。

4、设备系列上有常用 API 图面。

所有Windows 设备系列均使用相同的通用 Windows 平台 (UWP) 核心 API。如果你的应用仅使用核心 API，它将在任何 Windows 10 设备上运行。

5、扩展SDK可在专用设备上装饰你的应用。

扩展SDK可为每个设备系列添加专用 API。如果你的应用面向特定的设备系列，你可以使用这些 API 装饰该应用。在调用扩展 API 之前，通过检查应用在什么设备系列上运行，你仍然可以拥有一个在所有设备上运行的应用包。

6、自适应控件和输入

UI元素使用有效像素，因此它们会基于设备上可用的屏幕像素数自动自行调整。而且它们与多种输入类型（如键盘、鼠标、触摸、笔和 Xbox One 控制器）配合良好。 如果你需要进一步为特定屏幕大小或设备定制 UI，新的布局面板和工具将帮助你使 UI 适应运行应用的设备。

**UWP使用一种你已知道的开发语言**

你可以使用最熟悉的编程语言（如 C# 或 Visual Basic 和 XAML、JavaScript 和 HTML，或 C++ 和 DirectX 和/或 Extensible Application Markup Language (XAML)）创建通用 Windows 应用。你甚至可以采用一种语言编写组件，然后在采用另一种语言编写的应用中使用这些组件。

通用Windows应用使用Windows运行时，这是一个内置于操作系统的本机API。此API采用 C++ 实现，并支持 C#、Visual Basic、C++ 和 JavaScript，且对于每种语言都以非常自然的方式支持。

微软Visual Studio 2015为每种语言提供通用Windows应用模板，该模板允许你为所有设备创建单个项目。完成工作后，你可以生成应用包，并将其从Visual Studio提交到Windows应用商店，以在任何Win10设备上向客户提供你的应用。

相关资源：《<a href="https://msdn.microsoft.com/zh-cn/library/windows/apps/dn894631.aspx" target="_blank" rel="nofollow" >通用Windows平台 (UWP) 应用指南</a>》、《<a href="http://www.axiangblog.com/win10-visual-studio-2015-rtm.html" target="_blank" rel="nofollow" >Win10/安卓/iOS开发套件Visual Studio 2015正式版版官方下载</a>》