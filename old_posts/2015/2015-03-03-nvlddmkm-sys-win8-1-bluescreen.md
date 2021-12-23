---
id: 6704
title: nvlddmkm.sys Win8.1蓝屏莫慌 尽快升级至N卡GeForce 341.44公版驱动
date: 2015-03-03T22:04:46+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=6704
permalink: /nvlddmkm-sys-win8-1-bluescreen.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "13588"
cover:
  - ""
baidu_record:
  - "1"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:6705;s:11:"_thumb_type";s:10:"attachment";}'
smilie_vote_5:
  - "1"
smilie_vote_4:
  - "1"
categories:
  - Win10
  - Win8.1
  - 未分类
---
本周，阿象服役多年的老本G450 Win8.1平台意外遇到多次蓝屏和死机，蓝屏错误代码标记的也是神奇的英伟达的nvlddmkm.sys驱动程序，相信也有不少童鞋感同身受，那到底是怎么原因？

今天，阿象也前往Nvidia官方网站查询了相关型号显卡的最新驱动，发现了2015.2.24刚刚发布的GeForce 341.44驱动程序，官方说明表明分别为nvlddmkm.sys、nv4_mini.sys加入了安全更新，提升兼容性，估计旧版驱动程序会与第三方软件出现兼容性问题，最终导致出现蓝屏问题。

<a href="http://www.axiangblog.com/wp-content/uploads/2015/03/nvidia-bluesreen.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-6705" src="http://www.axiangblog.com/wp-content/uploads/2015/03/nvidia-bluesreen.jpg" alt="nvidia-bluesreen" width="450" height="207" /></a>下面，阿象也整理了GeForce 341.44 Win8.1、Win7两个平台的驱动程序下载包，如果你也遇到相同的蓝屏问题，不妨更新下N卡驱动试试。

**GeForce 341.44 Driver（2015.2.24）Win8.1专用**

本驱动更新为nvlddmkm.sys、nv4_mini.sys加入了安全更新，提升兼容性，可缓解第三方软件在Win8.1下与旧版显卡驱动兼容性蓝屏问题。

笔记本64位

http://cn.download.nvidia.com/Windows/341.44/341.44-notebook-win8-win7-64bit-international-whql.exe

台式机64位

http://cn.download.nvidia.com/Windows/341.44/341.44-desktop-win8-win7-winvista-64bit-international-whql.exe

**GeForce 309.08 Driver（2015.2.24）Win7专用**

本驱动更新为nvlddmkm.sys、nv4_mini.sys加入了安全更新，提升兼容性，可缓解第三方软件在Win7下与旧版显卡驱动兼容性蓝屏问题。

笔记本64位驱动

http://cn.download.nvidia.com/Windows/309.08/309.08-notebook-win8-win7-64bit-international-whql.exe

没有最好，只有更好的显卡驱动程序！