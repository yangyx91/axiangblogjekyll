---
id: 5306
title: 如何快速找回Win8.1/Win8.1 Update产品密钥，手动备份激活信息？
date: 2014-07-20T08:26:26+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=5306
permalink: /win8-1win8-1-update-key-backup.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
views:
  - "16234"
baidu_record:
  - "1"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:5305;s:11:"_thumb_type";s:10:"attachment";}'
love:
  - "1"
smilie_vote_1:
  - "1"
  - "1"
categories:
  - Win10
  - Win8.1
  - 未分类
---
之前，阿象为新用户分享了<a href="http://www.axiangblog.com/usb-hdd-disk-win7win8-1.html" target="_blank"  rel="nofollow" ><strong>U盘/硬盘全新安装Win7/Win8.1</strong></a>图文安装教程，也为高级用户准备<a href="http://www.axiangblog.com/dism-win8-1-update-os-backup.html" target="_blank"  rel="nofollow" >自己动手制作Win8.1出厂恢复镜像</a>等实用技巧。不过，对于部分用户来说，他们更倾向不定期重装Win8.1系统，这样可以解决各种系统问题，重头再来。 

不过，他们准备重装时才发现，原来早已忘记当初系统产品密钥（激活KEY），以及如何手动备份激活文件。所以，今天阿象就为这些&#8221;重装爱好者&#8221;送来这篇教程，帮助大家快速找回Win8.1/Win8.1 Update产品密钥，手动备份激活信息。 

**准备工具：  
** 

**ProductKey**（Win8.1 key查询工具，<a href="http://www.400gb.com/u/2574829/6731018" target="_blank"  rel="nofollow" >点击下载</a>）、**Win8.1激活备份还原工具**（由**jzsm**制作出品，<a href="http://www.400gb.com/file/68812331" target="_blank"  rel="nofollow" >点击下载脚本</a>） 

**具体教程如下：  
** 

1、下载运行ProductKey工具，这时将自动显示当前Windows产品密钥，即可手动复制该密钥，支持识别零售密钥、OEM密钥、Mak密钥； 

![](http://www.axiangblog.com/wp-content/uploads/2014/07/072014_0826_Win81Wi1.jpg) 

阿象注：我们可以使用slmgr.vbs /dlv命令，手动校验该工具提取的密钥是否正确。 

![](http://www.axiangblog.com/wp-content/uploads/2014/07/072014_0826_Win81Wi2.jpg) 

2、最后，我们比较了Win8.1/Win8.1 Update系统产品密钥，与该工具提取的密钥完全一致。 

![](http://www.axiangblog.com/wp-content/uploads/2014/07/072014_0826_Win81Wi3.jpg) 

<p style="margin-left: 5pt">
  3、现在，我们已成功找回Win8.1/Win8.1产品密钥，接着，就要手动备份Win8.1、Office2013的激活信息，具体只需运行<strong>Win8.1激活备份还原工具.bat脚本。</strong>
</p>

![](http://www.axiangblog.com/wp-content/uploads/2014/07/072014_0826_Win81Wi4.jpg) 

4、例如备份Win8.1激活文件，只需输入数字1，以及Win8.1产品密钥，即可完成备份，同时自动生成store文件夹。 

![](http://www.axiangblog.com/wp-content/uploads/2014/07/072014_0826_Win81Wi5.jpg) 

5、除了支持备份外，该脚本也支持还原Win8.1激活信息。 

![](http://www.axiangblog.com/wp-content/uploads/2014/07/072014_0826_Win81Wi6.jpg)