---
id: 9482
title: 全新JavaScript体验 微软Visual Studio 2017如何开启Salsa体验？
date: 2016-05-03T21:37:05+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=9482
permalink: /javascript-visual-studio-2017-salsa.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "3488"
baidu_record:
  - "1"
categories:
  - Asp.Net
  - Web开发
  - Win10
  - 未分类
---
四月初，微软推出了Visual Studio 2016预览版（代号：Visual Studio “15″）开发套件，主打轻量高效运行，同时首次加入「Salsa」全新JavaScript语言，值得开发者朋友一试。

据<a href="https://blogs.msdn.microsoft.com/msdntaiwan/2016/04/24/previewing-salsa-javascript-language-service-visual-studio-15-cht/" target="_blank"  rel="nofollow" >微软MSDN博客</a>介绍，Salsa为Visual Studio中的JavaScript语言做了许多强化，尤其是支持模块参考、完整的ES6/ES7语法以及JSX等等。

下载Visual Studio &#8220;15&#8221; 预览版ISO镜像：参考《<a href="http://www.axiangblog.com/win10-visual-studio-2016-iso.html" target="_blank"  rel="nofollow" >迎接Win10年度更新 微软开发套件Visual Studio 2016预览版官方中文ISO免费下载</a>》

**为什么需要一个新的语言服务？**

目前Visual Studio编辑JavaScript代码会为语言服务启动一个执行模型，基本上，当你输入一些程序代码时，背景有一个JavaScript引擎会不断执行你的程序代码，提供接近运行时间精准的语法提示列表、函数型态说明、以及其它的功能。  
<a href="http://www.axiangblog.com/javascript-visual-studio-2016-salsa.html/vs2016-salsa1" rel="attachment wp-att-9483" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9483" src="http://www.axiangblog.com/wp-content/uploads/2016/05/vs2016-salsa1.jpg" alt="vs2016-salsa1" width="450" height="183" /></a>这样的设计为语言服务这部份的功能带来更多的复杂度及不一致性。

所以，Salsa使用了与TypeScript用来推测对象型态相同的静态语言分析功能，透过这个新的语言服务，我们可以减少解决这些环境的问题；其次利用TypeScript可强化JavaScript代码的编辑体验，最后是支持更新的JavaScript语言标准，比如ES2016甚至是TypeScript以及往后的标准。

**如何在Visual Studio 2016“15″预览版中启用Salsa？**

复制以下代码，另存为salsa.reg，导入Win10平台，重启Visual Studio “15″即可生效。

**Windows Registry Editor Version 5.00**  
**[HKEY\_CURRENT\_USER\SOFTWARE\Microsoft\VisualStudio\15.0\TypeScriptLanguageService]**  
**&#8220;UseTypeScriptExperimental&#8221;=dword:00000001**

（注：开发者可以切换数值00000000为关闭、00000001为开启Salsa的功能）。

**Salsa所提供的“黑科技”新功能**

1、ES6以及CommonJS模块支持

Salsa已经能够处理ES6以及CommonJS模块的语法，这样一来我们便能跨模块提供 IntelliSense 的功能。

例如math-util.js：

/**  
* Returns square of a number.  
* @param {number} x Number to square.  
*/  
export function square(x) {  
return x * x;  
}

其它JavaScript脚本引入这个模块时，一样能够完成语法提示：

<a href="http://www.axiangblog.com/javascript-visual-studio-2016-salsa.html/vs2016-salsa2" rel="attachment wp-att-9484" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9484" src="http://www.axiangblog.com/wp-content/uploads/2016/05/vs2016-salsa2.jpg" alt="vs2016-salsa2" width="500" height="80" /></a>2、支持JSX语法

Salsa加入对JSX语法大量的支持，包括在JSX元素中语法上色以及自动完成，这些都大幅提升使用现代化使用JSX的开发框架（如：React)的程序代码编辑体验。

<a href="http://www.axiangblog.com/javascript-visual-studio-2016-salsa.html/vs2016-salsa13" rel="attachment wp-att-9485" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-9485" src="http://www.axiangblog.com/wp-content/uploads/2016/05/vs2016-salsa13.jpg" alt="vs2016-salsa13" width="500" height="313" /></a>  
3、从TypeScript定义中处理数据型态

这个新的语言服务核心也用来强化在Visual Studio中使用TypeScript的语言体验，Salsa也能利用大量由TypeScript社群所贡献的数据型态定义文件，其中包含了许多知名的JavaScript函式库及开发框架。

这些数据型态的信息以TypeScript定义档案的型式 (.d.ts 档案) 储存，Salsa就能够根据这些定义来处理JavaScript代码中的数据型态问题。

在默认的状况下，Salsa语言服务会尝试侦测使用的JavaScript函式库为何并且自动下载对应要参考的 .d.ts档案，想要了解更多这个功能的讯息，参考<a href="https://github.com/Microsoft/TypeScript/wiki/Using-the-Salsa-Preview-in-Visual-Studio-15-Preview#intellisense-based-on-typescript-definitions" target="_blank"  rel="nofollow" >GitHub</a>：

结语：Salsa的终极目标是提供一个可靠、用起来愉悦的JavaScript编辑体验，不过我们还有很多工作要完成才能达到这个目标。