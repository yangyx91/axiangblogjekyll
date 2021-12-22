---
id: 6462
title: Win10 TH2开发：Win10 SDK、Win10 Mobile 10586模拟器官方下载
date: 2015-11-11T21:46:13+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=6462
permalink: /win10-sdk-xaml-html5.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "22124"
cover:
  - ""
baidu_record:
  - "1"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:7074;s:11:"_thumb_type";s:10:"attachment";}'
smilie_vote_1:
  - "4"
smilie_vote_2:
  - "1"
smilie_vote_5:
  - "1"
categories:
  - Win10
  - Win10应用
  - 未分类
---
今年11月份，微软将为Win10平台推送秋季更新“Win10 TH2”，预计为Win10 Build 10.0.10586正式版，分别覆盖PC、平板以及手机平台，备受期待。现在，微软也为<a href="http://www.axiangblog.com/win10-visual-studio-2015-rtm.html" target="_blank" rel="nofollow" >开发套件Visual Studio 2015</a>玩家准备了最新Win10软件开发工具包 (Win10 SDK)、Win10 for Mobile模拟器，原生开发通用型Windows Apps。借助此预发行版Windows SDK，你可以开始构建跨平台Windows Apps应用和Win10桌面应用，当然此SDK也支持Win7、Win8.1等桌面应用程序。<!--more-->

<a href="http://www.axiangblog.com/wp-content/uploads/2015/10/win10-sdk.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-8254" src="http://www.axiangblog.com/wp-content/uploads/2015/10/win10-sdk.jpg" alt="win10-sdk" width="500" height="186" /></a>本款Win10 SDK实际版本号为10.0.10586，具体包含以下特色套件，参考如下：

相关文章：《<a href="http://www.axiangblog.com/dev-win10win10-mobile-10240.html" target="_blank" rel="nofollow" >Win10/Win10 Mobile 10240/10586仿真模拟器安装教程</a>》

1、Win10移动版仿真器（手机版Win10）

Win10移动版仿真器是一个桌面应用程序，它可以模拟运行Win10移动版（WP10）仿真器的设备。它提供了一个虚拟环境，你可以在其中调试并测试Windows App，而无需使用物理设备。它还为你的应用程序原型提供了独立的环境。

<a href="http://www.axiangblog.com/wp-content/uploads/2015/10/win10-sdk-mobile.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-8255" src="http://www.axiangblog.com/wp-content/uploads/2015/10/win10-sdk-mobile.jpg" alt="win10-sdk-mobile" width="500" height="211" /></a>

2、现在可通过GitHub获取Win10应用示例。

<a href="https://github.com/Microsoft/Windows-universal-samples/archive/master.zip" target="_blank" rel="nofollow" >https://github.com/Microsoft/Windows-universal-samples/archive/master.zip</a>  
这些示例专用于在支持 Universal Windows Platform 的桌面、移动设备和将来设备上运行。你可以在 MSDN 代码库中找到其他示例。

3、Windows SDK布局和元数据

该SDK包括用于标头、库和元数据的版本化文件夹。这将使将来版本的Win10 SDK 能够与之前的版本并行安装。

4、Windows合约

Windows运行时元数据不再保留在单个 Windows.WinMD 文件中。Windows 运行时元数据现在保留在 References 文件夹中的独立元数据文件中。合约文件通过各个平台的 Platform.XML 文件，以及各个平台扩展 SDK 所提供的 SDKManifest 文件加载。

5、Windows 平台扩展 SDK

Windows SDK包括以下平台扩展 SDK： Windows Desktop、Windows Mobile、Windows IoT 和 Windows PPI。当你将这些扩展添加到你的 Universal Windows App 项目时，特定于设备的 API 和元数据将可用于你的应用。这可以开启特定的功能，使用户体验变得个性化。

5、Unified C Runtime library (CRT)

Win10 SDK现包含了Microsoft Unified CRT &#8211; 一个在应用和操作系统之间共享的新 CRT。包含在该 SDK 中的标头、源和库使你可以通过该新 CRT 构建软件。

6、AllJoyn

AllJoyn 是一个允许设备发出信号并与其周围的其他设备共享功能的系统。此 SDK 包含了工具和库支持，以便你的应用可以使用 AllJoyn 标准与其他设备进行通信。

7、Windows App 认证工具包

Windows SDK中包含Windows 应用认证工具包 10 (Windows ACK)。使用ACK验证你的应用是否可以提交到Win7、Win8.1、WP8.1或Win10认证项目。

8、DirectX 更新

Win10 SDK引入了Visual Studio 2015中的Direct3D 12图形调试支持。新的Direct3D 12图形调试功能使你既能够在 Direct3D 11 中，又能够在 Direct3D 12 中无缝地调试图形。

现在可通过 DirectX 12 Early Access Program 获取最新的 Direct3D 12 示例、文档以及其他信息。获取有关 DirectX 的详细信息。

9、Windows性能工具包

Windows Performance Tools专用于分析各类性能问题，包括应用程序启动次数、启动问题、延迟的过程调用和中断活动（DPC 和 ISR）、系统响应能力问题、应用程序资源使用情况和中断攻击。

10、WinDBG和Windows调试器

Windows调试器可以在基于 x86、x64或ARM的处理器上运行，并且可以调试在基于x86、x64或ARM的处理器上运行的代码。该调试器和要被调试的代码有时在同一计算机上运行，但是其他时间该调试器和要被调试的代码在不同的计算机上运行。

11、AppVerifier

应用程序验证程序是一种用于本机代码的运行时验证工具，可以协助查找常规应用程序测试难以发现的细微编程错误。

12、Windows 辅助工具

之前随附在 Microsoft 辅助程序包 (MSAA SDK) 中的辅助工具现在将与 Windows SDK 一同提供。这些工具用于检查屏幕阅读器所使用的消息，以从应用程序获取文本，然后使用文本到语音转换朗读它，或将其传递给盲文设备。

13、.NET Framework 4.6 SDK

.NET Framework 是用于构建适用于 Windows、Windows Phone、Windows Server 和 Microsoft Azure 的应用的开发平台。它包含公共语言运行时 (CLR) 和 .NET Framework 类库，其中包括支持各种技术的类、接口和值类型。.NET Framework 提供托管的执行环境、简化的开发和部署，以及与包括 Visual Basic 和 Visual C# 在内的多种编程语言的集成。

阿象评：换句话，Win10 APP开发首选XAML语言，而HTML5+JS也将继续保留，作为候选语言而已，毕竟HTML5在统一平台方面的重要性也与日俱增！

**Win10 SDK 10.0.10586开发环境免费下载：<a href="http://pan.baidu.com/s/1dD9F2CT" target="_blank" rel="nofollow" >备份网盘</a>  
** 

<a href="http://download.microsoft.com/download/9/0/B/90B9A880-C3F8-43FB-B8F9-E4D4BFB5C85F/standalonesdk/sdksetup.exe" target="_blank" rel="nofollow" >http://download.microsoft.com/download/9/0/B/90B9A880-C3F8-43FB-B8F9-E4D4BFB5C85F/standalonesdk/sdksetup.exe</a>

访问Win10应用商店，<a href="https://dev.windows.com/zh-cn/downloads" target="_blank" rel="nofollow" >https://dev.windows.com/zh-cn/downloads</a>

**Win10 for Mobile 10.0.10586模拟器套件官方下载：<a href="http://pan.baidu.com/s/1dD9F2CT" target="_blank" rel="nofollow" >备份网盘</a>**

<a href="http://download.microsoft.com/download/6/D/6/6D6F6EB0-DB13-4590-9F0C-69A04127D1BC/emulator/EmulatorSetup.exe" target="_blank" rel="nofollow" >http://download.microsoft.com/download/6/D/6/6D6F6EB0-DB13-4590-9F0C-69A04127D1BC/emulator/EmulatorSetup.exe</a>

下载安装完成后，如果想看Win10 Mobile模拟器效果，磁盘文件flash.vhd默认安装路径是在C:\Program Files (x86)\Windows Kits\10\Emulation\Mobile\10.0.版本号.0文件夹里。

**Win8.1/Win10开发教程《HTML5+JS》**，<a href="http://pan.baidu.com/s/1dD9F2CT" target="_blank" rel="nofollow" >网盘下载</a>

支持Win8.1、Win10、Server 2012 R2等平台

范例教程：

<a href="http://www.microsoftvirtualacademy.com/training-courses/developing-universal-windows-apps-with-c-and-xaml?OCID=WIP_r_Jan_Body_Academy_16" target="_blank"  rel="nofollow" >http://www.microsoftvirtualacademy.com/training-courses/developing-universal-windows-apps-with-c-and-xaml?OCID=WIP_r_Jan_Body_Academy_16</a>