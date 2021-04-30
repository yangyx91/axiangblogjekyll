---
id: 6759
title: 简单粗暴！谷歌Chrome/火狐Firefox如何制作绿化免安装版
date: 2015-03-12T23:15:42+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=6759
permalink: /chrome-firefox-portable.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "6443"
cover:
  - ""
baidu_record:
  - "1"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:6763;s:11:"_thumb_type";s:10:"attachment";}'
smilie_vote_1:
  - "1"
categories:
  - Win10应用
  - 未分类
---
提到常用主流浏览器，不得不提到谷歌Chrome和火狐Firefox两位，当然也是很多技术爱好者、开发者日常测试和上网必备工具，目前，这两款浏览器已不约而同步入原生64位浏览器时代，性能更加强大。

近日，阿象无意中发现了Chrome、Firefox官方安装包均采用自解压机制，这也意味着我们可以简单粗暴制作一个“绿化”免安装版，第三方工具只需一个开源压缩软件7-zip 3.8，即可完成所谓的免安装绿色软件。

**谷歌Chrome 41官方下载**：<a href="https://www.google.com/chrome/browser/desktop/index.html" target="_blank" rel="nofollow" >传送门</a>、<a href="http://google.com/dl/chrome/win/E6D587340A678936/41.0.2272.89_chrome64_installer.exe" target="_blank" rel="nofollow" >离线包下载</a>、**火狐Firefox官方下载**：<a href="ftp://ftp.mozilla.org/pub/mozilla.org/firefox/releases/" target="_blank" rel="nofollow" >传送门</a>

操作方法：

首先安装下7-zip解压缩软件，建议普通用户使用64位Win8.1、Win7以上平台；

<a href="http://www.axiangblog.com/wp-content/uploads/2015/03/greensoft04.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-6763" src="http://www.axiangblog.com/wp-content/uploads/2015/03/greensoft04.jpg" alt="greensoft04" width="450" height="274" /></a>然后分别对Chrome、Firefox程序包直接解压提取核心安装目录，即可。例如火狐Firefox只需提取其中的“core”目录、谷歌Chrome需提取\chrome.7z\Chrome-bin完整目录。

<a href="http://www.axiangblog.com/wp-content/uploads/2015/03/greensoft01.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-6760" src="http://www.axiangblog.com/wp-content/uploads/2015/03/greensoft01.jpg" alt="greensoft01" width="450" height="270" /></a>最后，我们分别运行提取出来的目录中的chrome.exe、firefox.exe主程序，即可愉快的上网体验。

<a href="http://www.axiangblog.com/wp-content/uploads/2015/03/greensoft02.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-6761" src="http://www.axiangblog.com/wp-content/uploads/2015/03/greensoft02.jpg" alt="greensoft02" width="450" height="271" /></a>  
注：Chrome默认内置了Flash播放器，Firefox火狐浏览器需单独下载安装Flash播放器（<a href="http://www.adobe.com/go/getflash" target="_blank" rel="nofollow" >点击安装</a>）

<a href="http://www.axiangblog.com/wp-content/uploads/2015/03/greensoft05.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-6764" src="http://www.axiangblog.com/wp-content/uploads/2015/03/greensoft05.jpg" alt="greensoft05" width="450" height="273" /></a>  
**注：Chrome/Firefox浏览器配置、扩展、数据存储路径**

C:\Users\用户名\AppData\Local\Google\Chrome\User Data

C:\Users\用户名\AppData\Local\Mozilla\Firefox\Profiles

**如何加速Chrome/Firefox浏览器启动速度，优化数据库？**

这时只需配套使用Speedyfox即可（<a href="http://www.crystalidea.com/downloads/speedyfox.exe" target="_blank" rel="nofollow" >点击下载</a>）