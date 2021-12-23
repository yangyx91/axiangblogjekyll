---
id: 7622
title: Win10技巧：如何禁用Windows Defender各种计划任务？
date: 2015-08-12T07:51:25+08:00
author: yangyx91
layout: post
guid: http://www.axiangblog.com/?p=7622
permalink: /win10-windows-defender-disable.html
MOOD_COMMENT:
  - 's:115:"a:6:{s:4:"good";i:0;s:5:"great";i:0;s:5:"bored";i:0;s:8:"nonsense";i:0;s:13:"notunderstand";i:0;s:7:"passing";i:0;}";'
baidu_record:
  - "1"
views:
  - "9808"
tc-thumb-fld:
  - 'a:2:{s:9:"_thumb_id";i:7630;s:11:"_thumb_type";s:10:"attachment";}'
smilie_vote_2:
  - "1"
categories:
  - Win10
  - Win8.1
  - 未分类
---
不少Win7小伙伴发现，Win10版Windows Defender默认生成了4个计划任务，从而会导致Win10在每天特定的时间段，开始在后台对硬盘进行读写操作，完成相应的维护任务。

因此Win10对本地硬盘的读写会非常频繁，无论你是固态硬盘还是机械硬盘，既然知道了原因，那我们可以前往Win10的“任务计划程序库”，手动禁用这些项目，让硬盘君静一静。

<a href="http://www.axiangblog.com/wp-content/uploads/2015/08/win10-wd02.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-7629" src="http://www.axiangblog.com/wp-content/uploads/2015/08/win10-wd02.jpg" alt="win10-wd02" width="450" height="316" /></a>

操作如下：

1、打开此电脑，切换到顶部的菜单栏，打开管理；

<img loading="lazy" class="aligncenter size-full wp-image-7628" src="http://www.axiangblog.com/wp-content/uploads/2015/08/win10-wd01.jpg" alt="win10-wd01" width="450" height="321" /> 

2、依次定位系统工具》任务计划程序库》Microsoft》Windows》Windows Defender位置

<a href="http://www.axiangblog.com/wp-content/uploads/2015/08/win10-wd03.jpg" target="_blank"  rel="nofollow" ><img loading="lazy" class="aligncenter size-full wp-image-7630" src="http://www.axiangblog.com/wp-content/uploads/2015/08/win10-wd03.jpg" alt="win10-wd03" width="450" height="330" /></a>

3、这里我们将看到4项计划任务：Windows Defender Cache Maintenance（定期维护任务）、Windows Defender Cleanup（定期清理任务）、Windows Defender Scheduled Scan（定期扫描任务）、Windows Defender Verification（定期验证任务）

<img loading="lazy" class="aligncenter size-full wp-image-7631" src="http://www.axiangblog.com/wp-content/uploads/2015/08/win10-wd04.jpg" alt="win10-wd04" width="450" height="328" /> 

4、依次右击禁用这些计划项目，重启电脑生效，现在我们的硬盘君可以静一静了。

&nbsp;