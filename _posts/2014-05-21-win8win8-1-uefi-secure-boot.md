---
id: 4537
title: 想装Linux，先禁用Win8/Win8.1 UEFI安全启动
date: 2014-05-21T16:19:55+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=4537
permalink: /win8win8-1-uefi-secure-boot.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "5959"
category_icon:
  - "4226"
post_icon:
  - "4228"
baidu_record:
  - "1"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:5088;s:11:"_thumb_type";s:10:"attachment";}'
categories:
  - Win10
  - Win8.1
  - 未分类
---
不知不觉中，市面上大多数预装Win8/Win8.1的新电脑淘汰了传统BIOS，采用了全新UEFI启动引导机制。为了保证Win8/Win8.1系统安全，微软引入UEFI安全启动机制，默认只允许启动UEFI固件签名的系统。

虽然这项安全机制可以防止Rootkit类恶意软件，可以提供额外的安全层。不过该功能也存在一项缺点，可能阻止你在Win8新机器上双引导Linux。这次，我们也整理相应的操作流程，帮助系统爱好者禁用Win8/Win8.1 UEFI安全启动。

<!--more-->

<a href="http://www.axiangblog.com/wp-content/uploads/2014/05/win8.1-uefi.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5086" src="http://www.axiangblog.com/wp-content/uploads/2014/05/win8.1-uefi.jpg" alt="win8.1-uefi" width="450" height="202" /></a>

注：本文仅限于**英特尔、AMDx86架构平台，不适用ARM平台**。

具体操作流程如下：

1、登录当前Win8/Win8.1平台。平板用户只需轻扫屏幕右侧顶部，唤出Charm超级菜单；键鼠用户只需用鼠标移至桌面右侧顶部，或者使用“Win+C”组合键唤出Charm超级菜单；

<a href="http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW1.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5023" src="http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW1.jpg" alt="063014_1535_GhostW1.jpg" width="563" height="321" /></a>

2、选择设置，打开“更改电脑设备”；

<a href="http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW5.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5027" src="http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW5.jpg" alt="063014_1535_GhostW5.jpg" width="563" height="571" /></a>

3、Win8用户：只需进入**电脑设置**，打开**常规**，选择右侧的**高级启动**，点击立即**重新启动**：Win8.1用户：进入**电脑设置**，选择**更新和恢复；**

<a href="http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW6.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5028" src="http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW6.jpg" alt="063014_1535_GhostW6.jpg" width="563" height="303" /></a>

4、打开恢复，选择右侧的**高级启动**，点击立即**重新启动；**

5、这时Win8电脑将重新启动，进入如下界面，选择**疑难解答**；

<a href="http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW7.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5029" src="http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW7.jpg" alt="063014_1535_GhostW7.jpg" width="563" height="410" /></a>

6、继续选择**高级选项**；

<a href="http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW8.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5030" src="http://www.axiangblog.com/wp-content/uploads/2014/06/063014_1535_GhostW8.jpg" alt="063014_1535_GhostW8.jpg" width="563" height="416" /></a>

7、这时我们将看到**UEFI固件设置**，果断点击；

<a href="http://www.axiangblog.com/wp-content/uploads/2014/05/win8.1-uefi1.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5087" src="http://www.axiangblog.com/wp-content/uploads/2014/05/win8.1-uefi1.jpg" alt="win8.1-uefi1" width="450" height="254" /></a>

8、继续重启；

<a href="http://www.axiangblog.com/wp-content/uploads/2014/05/win8.1-uefi2.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5088" src="http://www.axiangblog.com/wp-content/uploads/2014/05/win8.1-uefi2.jpg" alt="win8.1-uefi2" width="450" height="254" /></a>

9、例如Surface平板UEFI固件页面下，我们只需将**Secure Boot Control**的**Enable**改为**Disable；**如果是桌面电脑，我们需要切换至Boot栏目，禁用**Secure Boot**功能，如下图所示，最后还要保存才能生效。

<a href="http://www.axiangblog.com/wp-content/uploads/2014/05/win8.1-uefi3.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-5089" src="http://www.axiangblog.com/wp-content/uploads/2014/05/win8.1-uefi3.jpg" alt="win8.1-uefi3" width="450" height="338" /></a>

现在，我们已成功禁用Win8/Win8.1 UEFI安全启动，然后就可以直接安装，引导Ubuntu等Linux系统。